# Sensitive Data / OUTLINE

|[Last Chapter - Monitoring and Auditing](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_07_Auditing) | [Back to the Table of Contents](https://johnborghi.github.io/Supporting_Scientific_Data/) | Next Chapter - Coming Soon |

## Chapter Summary

Be careful. This section deals with the special considerations that must be taken while working with certain types of data, including data that contains protected health information (PHI) and data that comes with restrictions on how and by whom it can be used.

This chapter is built on the principle that all data must be managed, but not all data necessarily needs to be shared (openly).

| [Principles of Good Data Management Practice](https://johnborghi.github.io/Supporting_Scientific_Data/supplements/SSD_good-dm-practice)| ["Good Enough" Practices in Data Management](https://johnborghi.github.io/Supporting_Scientific_Data/supplements/SSD_good-enough)|

# Module 03: Handling Sensitive Data

Special considerations must be taken while working with data that includes sensitive information. This module is built on the principle that managing research data requires managing risk.

| Key Points | Certain types of data require special consideration and treatment. Data is “sensitive” when it must be protected against unauthorized access and use. |
| :---- | :---- |
|  | Protection of sensitive data is not only a regulatory requirement, it is a core ethical requirement when conducting research. |
|  | The sensitivity of a dataset is not a binary judgement (sensitive vs non-sensitive), it is measured along a continuum of risk. |
|  | It is often useful to mitigate the risk of a given dataset through processes such as deidentification or anonymization. But these processes are often more complex than simply eliminating a column in a spreadsheet. |

## 8.1. Setting the stage for sensitive data

The year is 1997\. In the state of Massachusetts, the Group Insurance Commission (GIC) is responsible for purchasing health insurance for over 130,000 state employees and their families. GIC collects a huge amount of data, including details about hospital visits for each employee. After removing several “explicit identifiers” such as the patients’ names and social security numbers, this individual level data is then given to researchers upon request. Governor Bill Weld assures the public that, through the deletion of these identifiers, patient privacy is maintained. 

Latanya Sweeney, then a computer science PhD student, requests the GIC data and spends a small amount of money to buy the voter rolls of the city of Cambridge. As an experiment, she combines these two “de-identified datasets” and is able to identify Governor Weld in the GIC dataset. She then mails a copy of his health records to his office. Word of this experiment later reaches Washington D.C., where debate is underway about what would come to be known as the “Privacy Rule” of the Health Insurance Privacy Protection Act (HIPAA). 

## 3.2. What is sensitive research data?

Scientific data does not exist in a vacuum. Like the scientific research enterprise itself, data lies at the intersection of all manner of social and ethical considerations. As evidenced by the introductory anecdote, this chapter mainly focuses on issues related to **human subjects data** \- data from a living individual about whom an investigator is conducting research \- but consider the following situations:

* A research team is studying an endangered species (plant or animal). For the species to continue surviving, their location must be protected.  
* A research team is doing work involving classified information or trade secrets from a commercial partner. In order to access the data, the team had to sign a data use agreement restricting who can access it and for what purpose.  
* A research team is working with a set of data that they acquired after signing a data use agreement which stipulates who can access the data and what they can use it for.

**Sensitive data** refers to data that must be protected against unauthorized access and use. As will soon be evident, *unauthorized* is doing quite a bit of work in this definition.

Properly managing sensitive data requires navigating intersecting technical and regulatory requirements. This chapter will also cover forms of sensitive data encountered by researchers working with data from cell lines, tissues, animal models and other sources. But to begin a deeper dive into the world of sensitive data, we will begin with a discussion of research involving human subjects.

In the United States, the federal government defines **research** as “systematic investigation, including research development, testing and evaluation, designed to develop or contribute to generalizable knowledge.” This definition may seem a little rudimentary, but sensitive data is an area in which key terms have very precise definitions. To this end, a **human subject** is an “individual who is or becomes a participant in research, either as a recipient of the test article or as a control.”

These definitions are quoted from the Federal Policy for the Protection of Human Subjects (also called the **Common Rule**), the baseline standard of ethics for government-funded research in the United States. Regardless of funding source, most US-based institutions actually hold their researchers to the terms laid out by this policy. Core to the Common Rule are the following ethical principles, originally outlined in Belmont Report (see **Table 8.1.** below).

**Table 8.1. Ethical principles outlined in the Belmont Report**

| Respect for Persons | Incorporates at least two ethical convictions individuals should be treated as autonomous agents Persons with diminished autonomy are entitled to protection This principle encompasses concepts such as informed consent and the protection of vulnerable populations |
| :---- | :---- |
| **Beneficence** | Persons are treated in an ethical manner not only by respecting their decisions and protecting them from harm, but also by making efforts to secure their well-being. This principle encompasses concepts such as minimizing risks while maximizing benefits. |
| **Justice** | Research subjects should be selected fairly and that the risks and benefits of the research should be distributed equitably. This principle encompasses concepts such as the fair distribution of burdens and benefits. |

So how does all this relate to sensitive data and Good Data Management Practice?

Research ethics, including the principles outlined in the Belmont Report, must be centered in all aspects of the research process. Protecting human subjects means, among other things, protecting their private information. 

**Private information** falls into two categories:

1. Information about behavior that occurs in a context in which an individual can reasonably expect that no observation or recording is taking place.  
2. Information which has been provided for specific purposes by an individual and which the individual can reasonably expect will not be made public.

Medical records are often used as an example of private information and certainly medical records are a source of data in many research studies. But the proper management of private information is vital for any research involving human subjects. 

At this point a careful reader may be wondering how the protecting private information from human subjects squares with research data sharing. If data needs to be protected, how can it be made available for use by others? This is an ongoing discussion, but among the missing pieces is the *identifiability* of the data. 

**Personally identifiable information (PII)** is information that can be used to distinguish or trace an individual’s identity, either alone or in combination with other information that is either linked or linkable to that individual. A research subject’s name is an obvious example of PII, as is information like their social security number. But less directly identifiable information can also be PII. On their own, data points like an individual’s gender identity, their zip code, and their birthday may not be enough to identify them. But, as shown in this chapter’s introductory vignette, reidentification becomes much easier with all three[^1].

### 8.2.1. Regulations and Expectations

For biomedical research occurring in the United States, it is not uncommon for sensitive data to be discussed in terms of the **Health Insurance Portability and Accountability Act (HIPAA)**. This regulation provides national standards for the protection of certain sensitive health-related information and establishes an individual’s rights over their health data. Among HIPAA’s is the notion that some information about an individual is particularly sensitive. HIPAA lists eighteen examples of such information, which are detailed in **Table 8.2.** below.

When identifiable information is linked to information related to the health status, provision of health care, or payment for health care for an individual it can become **protected health information (PHI).** PHI is broadly defined as information that can be linked to a particular person that is generated in the course of providing a health care service. PHI can be found in medical records, payment records, insurance information, clinical test results, medical images, wellness and disease management program files, clinical case notes, and many other sources of data.

Though the identifiers listed in **Table 8.2.** are often colloquially called the HIPAA identifiers, it is important to note that this list is not meant to be exhaustive. This list provides illustrative *examples* of the information that must be removed from a record or dataset in order for it to not longer be  considered PHI. Adding to this complexity, information can also be considered PII at one point in time and then turn into PHI later, as it is linked to health-related information.

**Table 8.2. HIPAA Identifiers**

|  | Identifier |
| :---- | :---- |
| 1 | Name |
| 2\* | Address (all geographic subdivisions smaller than state, including street address, city county, and zip code). |
| 3\* | All elements (except years) of dates related to an individual (including birthdate, admission date, discharge date, date of death, and exact age if over 89\) |
| 4 | Telephone numbers |
| 5 | Fax number |
| 6 | Email address |
| 7 | Social Security Number  |
| 8 | Medical record number |
| 9 | Health plan beneficiary number |
| 10 | Account number |
| 11 | Certificate or license number |
| 12 | Vehicle identifiers and serial numbers, including license plate numbers |
| 13 | Device identifiers and serial numbers |
| 14 | Web URL |
| 15 | Internet Protocol (IP) Address |
| 16 | Finger or voice print |
| 17 | Photographic image \- Photographic images are not limited to images of the face. |
| 18 | Any other characteristic that could uniquely identify the individual |

Please note that the 18 HIPAA identifiers are *examples* of the information that must be removed from a record or dataset in order for it not to be considered PHI. HIPAA was passed several decades ago, which accounts for the incomplete nature of this list. Plus, who even has a fax machine? Information can also be personally identifiable at one point in time and then turn into PHI later, as it is linked to health-related information.

There is a lot of confusion about what HIPAA does and does not cover. What is most relevant in the context of Good Data Management Practice is that data that includes PHI has must be stored and shared in line with very specific regulatory requirements. More on these later.

HIPAA is not the only regulation that applies to sensitive research data or data from human research subjects. The United States does not have a single federal privacy law, but rather a collection of sector-specific and state specific laws. For example, research involving student data in the United States intersects with regulations like the *Family Educational Rights and Privacy Act (FERPA)* and the collection of data from children using online tools falls under the *Children’s Online Privacy Protection Act (COPPA)*. Different states even have different regulations, such as the *California Privacy Rights Act*.

Of course, neither research nor privacy rights are constrained to just the United States. In fact, outside of the U.S., protection of private information is often regulated by much broader legislation.

The **General Data Protection Regulation (GDPR)** deals with the protection of personal data for individuals living in the European Economic Area (EEA), which covers countries in the European Union, Iceland, Liechtenstein, and Norway[^2]. Similar to the definition of “private data” in US-based regulation, GDPR defines personal data as any information that relates to an identified or identifiable living individual who is physically located in the EEA. Certain types of personal data, such as data related to an individual’s health, genetics, demographic or cultural characteristics, or biometrics, are regarded as “special cases” because of their potential to violate an individual’s privacy. 

The main rights granted to individuals under GDPR are outlined in **Table 8.3.** Please note that, in the parlance of GDPR, *processing* refers to any action performed on personal data, including those related to its collection, use, and deletion.

**Table 8.3. Rights conferred by GDPR**

| Right | Description |
| :---- | :---- |
| The right to be informed | Individuals have a right to be informed when their data is going to be processed  |
| The right of access | Individuals have a right to access their personal data and receive a copy of it. |
| The right to rectification | Individuals have a right to have inaccurate or incomplete personal data corrected. |
| The right to erasure | Individuals have a right to request the deletion of their personal data (under certain circumstances). This is often called the **right to be forgotten.** |
| The right to restrict processing | Individuals have the right to request that their personal data not be processed (under certain circumstances) |
| The right to data portability | Individuals have the right to obtain and then reuse their personal data for their own purposes across different services. |
| The right to object | Individuals have the right to object to the processing of their data for specific purposes (e.g. marketing). |
| Rights related to automated decision making including profiling | Individuals have the right to request human intervention in decisions otherwise based on automated processing of their personal data. |

These rights affect everything from how data is collected to how (and for how long) it can be stored. But GDPR is not meant to impede research. Personal data can still be collected and used as part of scientific research and exemptions to the strictest interpretations of the rights above are allowed in a research context as long as the appropriate safeguards are in place and there is an accounting of the proportionality and necessity of the exemptions. Researchers collecting or storing data in jurisdictions where GDPR applies should make sure they are aware of these issues.

**8.2.2. Contracts and Agreements**

The previous subsection is in no means comprehensive. At a given research institution, there are likely policies and procedures related to sensitive research data that intersect with local, national, and international regulations and expectations. But the terms dictating how a sensitive set of research must be handled are not just set by regulation. If a set of sensitive information is shared between two organizations \- such as researchers at one university sharing sensitive data with researchers at another university or company \- then there are contractual obligations as well.

A **data use agreement (DUA)** is a contract that establishes who is permitted to receive a specific dataset, how it may be used, and how it must be protected. A DUA must be completed BEFORE any exchange of sensitive data can take place. While they must abide by them, researchers should not engage with DUAs on their own. Understanding, developing, negotiating, and signing DUAs should be done in collaboration with the appropriate administrative team within a research organization.

## 8.3. Risk and research data

Thus far, this chapter has mostly focused on the sensitivity of research data in terms of very broad categories \- data that is sensitive versus data that is not sensitive. But, like most things, the reality of sensitive data is a good deal more complex.

In the context of Good Data Management Practice, **risk** is defined as the extent to which an organization or individual could be adversely affected by an event related to research data. 

In general, the risk of a particular event is calculated based on its likelihood and consequences.

* **Probability** \- The chance that an event will occur.   
* **Severity** \- The seriousness of the outcome if the event occurs.

Note the breadth of these definitions. Due to the mishandling of data, an individual research participant may risk their private information becoming public, a research team may risk disciplinary action or other professional consequences, a research institution may risk substantial fines and reputational damage. All of which is to say, making sense of and managing risk requires answering some fundamental questions.

**Risk to Whom?**

The first question is **“*Risk to whom?*”** A research organization and a research participant face different forms of risk. Consider the following examples.

*A research team is conducting a high profile study in which students at an academic institution are asked to complete surveys on a number of delicate topics. The data is anonymized at the point of collection, meaning there is no way for anyone to connect survey responses back to any individual on campus. The institution’s IRB has also determined that the research team  has both implemented every measure possible to mitigate any distress participants may feel as a result of their participation and will be providing sufficient resources and support after the fact.*

*Unfortunately, the team does not have a well-developed standard operating procedure for saving and backing up data. After the publication of a highly publicized article describing their results, the team discovers that they cannot establish data provenance. They eventually volunteer to retract their article.*

In this example, every effort was made to minimize risk to the participants and, with the exception of suboptimal data management, everyone did everything right. But this situation still represents a risk, the research team had to retract their article. The standing of the organization as an established site of careful and sound research may be diminished. This sort of situation represents a **reputational risk**.

*A research team is working with data that was derived from the electronic health record (EHR) of a hospital associated with their institution. Before the data was transferred to them, the hospital redacted patient names but, because of the team’s research questions, left other information \- such as their hospital admission and discharge dates and birthdates \- intact.*

*To test a new computational workflow, a member of the team uploads some of the data to a public Github repository. The researcher later states that they believed that, because the data no longer contained the names of the participants, it was anonymous. The researcher was overdue on their training related to working with data from human subjects.*

This example includes risk to both the research participants (i.e. the patients whose data was shared with the research team) and also the organization. The risk for the participants is, of course, that their private data is now public. For the organization, this situation represents a **compliance risk.** Because the data includes protected health information, this situation represents, at the very least, a violation of HIPAA. After an investigation by the U.S. Department of Health and Human Services' Office for Civil Rights, the organization may face fines and potentially other corrective actions.

Risk to an organization is not unrelated to risk to participants. When participating in research, participants may be exposed to psychological, social, and even physical risks. These do not always directly relate to Good Data Management Practice, of course. If a participant is negatively affected by the questions posed in a questionnaire, that is a question of research design rather than data management. But data management is essential when dealing with **informational risk** \- the potential for harm or other negative impacts due to the misuse, unauthorized access, or disclosure of information from a participant's involvement in a research study. If the content of that survey is such that a breach in confidentiality or privacy could place the participant at a physical or social risk, then that data must be considered sensitive and treated as such.

**Levels of Risk**

Adequately addressing all of this requires answering a second question: **“What is the risk level?”** Many research organizations use risk-based categories for research data. Such categories then determine what procedures must be implemented to protect the data, including specifics about how the data must be stored and what sorts of permissions are needed for access. Organizations differ in terms of their categorizations, but generally such systems resemble something like the one presented in **Table 8.5.** Below.

| Level | Description | Example |
| :---- | :---- | :---- |
| Low Risk | Data for which there would be little to no impact if it were compromised (subject to unauthorized access), lost, or destroyed. Often this type of data is labelled as *unrestricted* or *public*. | Data from a project involving tracking the eye movements of model organisms as examine a visual scene. |
| Moderate Risk | Data for which there would be a negative impact if it were compromised, lost, or destroyed. However the impact would not be severe for either research participants or the research organization. Such data is not generally available to the public, but there is no law or regulation outlining how it must be secured. | Data from a project in which human research participants were asked to complete a mental math task. The dataset does not contain the names of the participants and may contain limited information about them (e.g. their gender identity, the year they were born, questionnaire scores).  |
| High Risk | Data for which there would be a severely negative impact if it were compromised, lost, or destroyed. Typically, the governance of this type of data is required by a law or regulation (i.e. HIPAA) | Data from a project in which human research participants were asked to participate in a randomized controlled trial of a pharmaceutical intervention. The dataset contains information about each participant’s health status and other protected health information. |

When it comes to research data, researchers should not assess risk all on their own. This is not meant as a slight or a criticism. But rather an acknowledgement that information security is a whole world unto itself. For example, without delving too much into the world of cybersecurity policy, there are very specific requirements for systems that deal with data that contains PHI and other forms of sensitive information (i.e. SP 800-171 in the United States). The process of risk assessment \- which involves systematically identifying and estimating risks \- should be collaborative, involving the requisite units and expertise at a researcher’s home instituytion. 

## 8.4. Mitigating Risk

There are often ways to reduce the sensitivity of a dataset. Note the use of *reduce* rather than *eliminate*. Especially for data related to human subjects, risk is a moving target. This se

Adequately protecting sensitive data is often presented as a cybersecurity problem. This is for a good reason, not every system is appropriate for storing and managing sensitive data. Even a system that requires credentials to access and use (e.g. a username and password) may not be secure enough for data categorized as high risk. Such data is often described as “restricted” or “regulated” due to the rules and regulations governing how it must be stored. Substantial information technologies resources are expanded at research institutions across the world to establish compliant systems. 

For the purposes of Good Data Management Practices, being a cybersecurity policy expert is less important than. But, on their own, even the most sophisticated cybersecurity systems are insufficient when handling sensitive data. At the end of the day, Good Data Management Practice comes back to practices and strategies. The same is true for sensitive data.

**The Practice of Safely Handling Sensitive Data**

Cybersecurity is not the whole story, it is an important part of the story. To adequately address compliance with applicable regulations (and ensure they remain on good terms with their local research administrators and information technologists) researchers should always verify that the systems they intend to use to handle data are suitable for that data. This determination should happen very early in the research process, before data is collected.

Very often an organization will have tools for handling low and moderate risk data that should not be used with high risk data and vice versa. Because of the nature of these systems, it is not really possible in a guide like this to recommend one specific tool over another, just **please ensure that data is being stored on the appropriate systems.**

With the appropriate technical systems in place, the next step is to ensure the appropriate practices are also in place. Circling back to Documentation, this is where having a robust set of standard operating procedures becomes essential.

**Education, Standardization, Auditing**

Anyone who has ever worked in research has probably (hopefully) had to complete some training in cybersecurity. Usually this involves learning about institutional policies and resource and some very high level do’s and don’ts: Do use secure storage platforms, don’t lose your unencrypted laptop full of high risk data. But, during the actual practice of research, research teams are, more often than not, in a position where they need to develop their own specific protocols and procedures.

In addition to using the appropriate systems, adequately protecting sensitive data also requires implementing the appropriate practices. That means developing, implementing, and verifying a robust set of standard operating procedures related to management of sensitive data. As discussed in the chapter on documentation, it is also essential that these procedures be checked regularly to ensure that they are being implemented properly.

**Deidentification and Anonymization**

A common method for managing sensitive data is to reduce its risk through processes like de-identification, masking, and anonymization. These terms are defined or more precisely below, but generally refer to processes through which information is removed or changed to reduce the riskiness of a dataset.

* **Masking** \- The process of modifying a dataset to obfuscate sensitive information.

* **Deidentification** \- The process of altering information within a dataset in order to remove personally identifiable information (PII). Sometimes is used to refer to situations in which the identifying information can be re-linked to the rest of the data.  
    
* **Anonymization** – The process of removing information from a dataset in order to prevent re-identification. Sometimes is used to refer to situations in which the identifying information is permanently severed from the rest of the data.   
  * **Pseudonymization** refers to processes by which directly identifiable information is removed from a dataset, but an individual may still be identifiable by combining other information from the dataset (i.e. indirect identifiers).  
    

It is important to note that there is not a universal method for ensuring deidentification or anonymization. In practice, these terms are based more on regulation than on mathematical guarantees of anonymity. To illustrate this point, here are two methods outlined by HIPAA for deidentifying a dataset.

* **Safe Harbor** \- In the strictest interpretation, this requires the removal of all of the identifiers listed in table 8.1. from the dataset. A dataset that retains dates referring to a person, location information, and/or and age-related information is known as a “limited dataset” and is still considered PHI, but can be disclosed \- under certain conditions \- without a patient’s authorization.  
    
* **Expert Determination** \- Requires the attestation from a person with appropriate knowledge and experience that accepted statistical and/or scientific principles and methods for rendering information not individually identifiable have been implemented.

Definitions

**Anonymization** – The process of removing information from a dataset in order to prevent re-identification. **Pseudonymization** refers to processes by which directly identifiable information is removed from a dataset, but an individual may still be identifiable by combining other information from the dataset (i.e. indirect identifiers).

**Common Rule \-** The baseline standard of ethics for government-funded research in the United States. Regardless of funding source, most US-based institutions actually hold their researchers to the terms laid out by this policy.

**Deidentification** \- The process of altering information within a dataset in order to remove personally identifiable information (PII). 

**Data use agreement (DUA) \-** A contract that establishes who is permitted to receive a specific dataset, how it may be used, and how it must be protected. A DUA is needed whenever sensitive data is shared between organizations.

**Expert Determination** \- Requires the attestation from a person with appropriate knowledge and experience that accepted statistical and/or scientific principles and methods for rendering information not individually identifiable have been implemented.

**General Data Protection Regulation (GDPR) \-** A data privacy law regulating how personal data can be handled within the EU and European Economic Area (EEA).

**Health Insurance Portability and Accountability Act (HIPAA)** \- A U.S. federal law regulating the protection of sensitive patient health information.

**Human subject** \- An individual from or about whom data is collected in research. For example, they may be the recipient of a test or act as a control.

**Human subjects data** \- Data from a living individual about whom an investigator is conducting research.

**Masking** \- The process of modifying a dataset to obfuscate sensitive information.

**Personally identifiable information (PII)** \- Information that can be used to distinguish or trace an individual’s identity, either alone or in combination with other information that is either linked or linkable to that individual. 

**Private information** falls into two categories:

1. Information about behavior that occurs in a context in which an individual can reasonably expect that no observation or recording is taking place.  
2. Information which has been provided for specific purposes by an individual and which the individual can reasonably expect will not be made public.

**Protected health information (PHI) \- I**nformation that can be linked to a particular person that is generated in the course of providing a health care service.

**Safe Harbor** \- In the strictest interpretation, a method of deidentification that involves the masking of all “HIPAA identifiers” from a dataset.

**Sensitive data** \- Data that must be protected against unauthorized access and use.

**Research** \- For the purposes of complying with related policies and regulations, an effort is considered research if it includes the following elements.

1. It is a systematic investigation, including research development, testing and evaluation  
2. It is designed to develop or contribute to generalizable knowledge.

This definition is intentionally narrow for regulatory purposes, and does not mean that other efforts are not research.

**Risk \-** The extent to which an organization or individual could be adversely affected by an event related to research data. Risk is calculated based on the chance that an event will occur (**probability)** and the seriousness of the outcome if the event occurs (**severity**) and can take different forms, including reputational risk, compliance risk, informational risk, etc.

[^1]:  This is getting progressively easier with advances in AI and machine learning. See: Rocher, L., Hendrickx, J. M., & De Montjoye, Y.-A. (2019). Estimating the success of re-identifications in incomplete datasets using generative models. *Nature Communications*, *10*(1), 3069\. [https://doi.org/10.1038/s41467-019-10933-3](https://doi.org/10.1038/s41467-019-10933-3)

[^2]:  Since leaving the European Union, the United Kingdom has retained the provisions of GDPR in legislation called UK-GDPR.
