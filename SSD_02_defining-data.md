# Defining Research Data

|[Last Chapter - Understanding Data Management](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_02_defining-data) | [Back to the Table of Contents](https://johnborghi.github.io/Supporting_Scientific_Data/) | [Next Chapter - Planning for Data Management (https://johnborghi.github.io/Supporting_Scientific_Data/SSD_03_Planning) |

## Chapter Summary

Data is more than just an individual file or set of measurements. This chapter details how to understand all of the components of data as situated within a research workflow. 

This chapter is built on the principle that effective data management requires research data to be defined thoroughly and broadly.

| [Principles of Good Data Management Practice](https://johnborghi.github.io/Supporting_Scientific_Data/supplements/SSD_good-dm-practice)| ["Good Enough" Practices in Data Management](https://johnborghi.github.io/Supporting_Scientific_Data/supplements/SSD_good-enough)|

| | **Key Points for this Chapter** |
| :---- | :---- |
| 1\. | In the context of data management, a research workflow can be considered the series of steps that are implemented to reach a research finding. |
| 2\. | Research data is more than just individual objects or files. All the information, materials, and documentation needed trace a research workflow count as data. |
| 3\. | An individual researcher (probably) does not own the data they work with, but they (probably) have a lot of related rights and responsibilities. |
| 4\. | Taking care of data also means considering where it comes from and what it will be used for, not just within a given research project but also within the broader context of power and self determination. |

## 2.1. What is Research Data?

Before getting into more practical activities related to data management and sharing, it would be prudent to address a fundamental question \- What are we talking about when we talk about research data?

This may seem like a simple or even absurd question, but defining and understanding research data is an essential first step in thinking through data management and sharing-related practices and strategies.

To start us off, here is the definition of scientific data given by the National Institutes of Health in their Data Management and Sharing Policy[^1]:

*“Scientific data is the recorded factual material commonly accepted in the scientific community as of sufficient quality to validate and replicate research findings, regardless of whether the data are used to support scholarly publications.”*

Stated a bit more simply, **research data** can be thought of as the materials and information that supports a research result.

Note that this a bit different than definitions of data used in coversations related to data storage and organization. That distinction is explored in-depth in the eponymous chapter.

The next question is, of course, what is meant by “support”? 

For a given research result, consider the answers to the following four questions:

1. What information underlies this result?  
2. Where did that information come from?  
3. How did the researchers involved get from this information to the result?  
4. What would be needed for other researchers in the same field to potentially get the same result from the same information?

Every file, script, piece of documentation, and other research-related object or material that comes up as an answer to any of these questions can be considered as research data.

Not all of it needs to be saved forever, but all of it needs to be effectively managed.

>**Example:** Behavioral Data Collection  
>
>A research team is conducting a project which involves human participants completing a memory test on a computer. For each participant, response accuracy and reaction time are recorded automatically for each participant. Participants are also asked to complete several questionnaires. To analyze the data, the researchers must clean the data collected from the individual participants, then calculate average or aggregate values for each (e.g. overall response accuracy for each participant, average reaction time for each participant), then run the requisite statistical tests. 
>
>*What is the data that needs to be managed?*
>
>The above example is extremely straightforward as a research project, some variant of this design is currently being run in many psychology research labs across the world. 
>
>But what “counts” as the data? 
>
>Here is a non-exhaustive list. 
>
>* The code/software that was used to present the test to the participants and record their responses. 
>* The output files that contain information about each participant’s accuracy and reaction time to each prompt on the task. 
>* Files containing each participant’s questionnaire responses. 
>* The files that contain the cleaned data about each participant’s response accuracy and reaction time to each prompt, questionnaires, etc. 
>* The documentation that describes how each individual-level data file was cleaned and/or the code or scripts that were used to clean the data. 
>* The files that contain the averaged and aggregated data for all of the participants together. Possibly versioned. 
>* The code/software used to analyze the data. The documentation that describes how the data were analyzed (e.g. lab notebooks). A “final” dataset that contains the information that supports a set of research findings. 
>
>All of these items need to be properly managed but, even under the most open definition of the term, most of them will not need to be shared. 

## 2.2. The Research Workflow

During the day-to-day course working in scientific research, it can be tempting to think about research data in terms of individual files or objects. 

A very large percentage of researchers have probably, at some point, created a file and named it something like *data.xls*. But this belies the tremendous breadth and heterogeneity of the objects and information that need to be effectively managed when working in twenty first century research. For even the most straightforward of projects, defining data is not that simple.

A set of data can include quantitative observations recorded in an Excel file or a set of images of recordings of a semi structured interview.It could include information a research team collected or generated themselves to answer a specific research question or information collected by others that is being repurposed. Depending on the type of research being conducted, data can take just about any form imaginable. But it is still not that simple. 

Data is acquired, processed, analyzed, and communicated under specific circumstances. Choices and assumptions are made at every step and smallest details can have substantial consequences. Research is a process and it is unlikely that an individual file or object could contain all of the information necessary to fully examine, replicate, and extend that process.

For this reason, it is useful to consider research data within the framework of a **research workflow**. Stated simply, a workflow is the series of steps that are implemented to reach a research finding. There are multiple points in any research effort where decisions are made that can significantly affect the final result. A research workflow (also sometimes called a “pipeline”) traces the steps a research team *actually* takes among many possibilities and directions not taken. In the context of managing and sharing research data, everything needed to reconstruct a research workflow can be considered as data. 

| <img width="800" alt="Image" src="https://github.com/user-attachments/assets/6e653223-915f-4c18-8ada-205d3e4a40e3" /> |
| ----- |
| **Figure 2.1.**  This is not your data. The measurements or information that are included in your data were not generated or analyzed in a vacuum. All of the information and materials needed to reconstruct a research workflow can be considered as data. |

Research workflows are conceptually similar to the notion of data provenance discussed in the first module as well as visualizations such as the **research data lifecycle** that are commonly cited in the data curation community[^2]. What unites these models is the understanding that management of research data is a continuous process, occurring over course of a research effort.

Certainly the “course” of a research is not always linear. Very rarely does it proceed in discrete phases or stages. But as is shown in Table 2.01., different data management activities are implemented at different time points. As with activities related to the collected analysis of data, decisions made at earlier time points related to how data is managed can substantially affect what can be done later.

As stated in section 2.01, a broad, workflow-based definition of research data includes both the objects and information that actually underlie a set of research results (e.g. Excel files containing test scores, images, etc) but also the information needed to understand, evaluate, and make use of those objects. That is, metadata.

The term **metadata** generally refers to information *about* a piece of data. Metadata may describe, explain, or facilitate the use of an element of the data (e.g. a specific file) or the dataset as a whole. For some forms of research data, formal metadata standards or schemas have been developed that precisely specify how different characteristics of the data should be described and organized. However, the term can also be used to refer more generally to documentation (e.g. readme files, data dictionaries, protocols, lab notebooks) that are created and maintained by the research team to facilitate the use of a dataset. 

The module covering documentation covers this in much greater detail but, in the context of data management and sharing, metadata should be considered “part” of research data.

Throughout this guide we’ll return to our expansive and workflow-based definition of data for several reasons:

1. Ideally, a research workflow is planned in advance and builds toward fulfilling the goals of the research effort. Incorporating data management into research workflows helps incorporate related practices into the day-to-day routine of doing research rather than “extra work” to be done after the fact.   
2. This definition helps to emphasize that data management is about data and other materials that are *in process,* meaning that they are acquired, processed, analyzed, archived, and shared in order to be acted upon in some way. 

` All of the information and materials needed to reconstruct a research workflow can be considered data. `

| <img width="800" alt="Image" src="https://github.com/user-attachments/assets/e3cc3bab-e933-47d8-956f-e43b72e511a3" />|
| ----- |
| **Figure 2.2.**  A representation of the research workflow. There are multiple points in any research effort where decisions are made that can significantly affect the final result. A research workflow (also sometimes called a “pipeline”) traces the steps a research team *actually* takes among many possibilities and directions not taken.  |

## 2.3. Categories of Research Data

Just as introductory statistics classes distinguish between nominal, ordinal, interval, and ratio values in quantitative data (see this primer for a refresher, if needed), distinguishing between different “types” of research data can be helpful in determining the precise data management practices that need to be implemented.

Two major ways to categorize data “types” are through their format and their size. Often, data will be described as quantitative or qualitative, depending on if information is counted or measured using numerical values. Scientific data can also be categorized as “big” versus “small”, depending on if it is too complex or has too high a volume to be of use with commonly used software tools.

But scientific data comes in so many formats \- spreadsheets, images, medical records, interview transcripts, text files, information recorded on paper, and so many others \- that tackling them all individually is beyond the scope of this guide.

So it might be helpful to take a step back.

Throughout a research workflow, it is possible to talk about data as falling into several categories based on time point or degree of processing. These categories are described in **Table 2.1**.

#### Table 2.1: Stages of Research Data

| Stage | Description |
| :---- | :---- |
| Raw Data | The “original observations” taken directly from a source. |
| Intermediate Data | Forms of data within a research workflow that did not exist before the workflow began and may not be maintained once a “final” dataset has been completed. |
| Final Data | The dataset that most directly underlies a set of research findings. |

These categories are not necessarily discrete or meant to account for every category of data used by every research team everywhere. An essential characteristic to consider when setting up a set of management practices around a set of data is its source.

This is expanded upon in **Table 2.2**.

#### Table 2.2: Categories of Research Data

| Data Type | Description | Examples |
| :---- | :---- | :---- |
| Primary Data | Data collected, processed, and analyzed by a research team to address specific research questions. | A research team collects measurements from model organisms to address their hypotheses. Another research team conducts a clinical trial in which they test the efficacy of an intervention on two groups of participants. |
| Repurposed or Secondary Data | Data collected for one purpose and subsequently repurposed, aggregated, curated, and/or provisioned to be re-used for another. | A research team uses clinical data from the electronic health record at Stanford Healthcare to examine trends over time. Another team uses insurance claims data acquired and curated by Population Health Sciences. |
| Simulated or Synthetic Data | Data synthesized through a stochastic process to  augment or replace real world data. | A research team generates a set of synthetic data to help improve their artificial intelligence models. Another research team synthesizes a set of data based on the characteristics of a highly sensitive dataset they have used to draw a set of conclusions. They share the synthetic data to address reproducibility-related issues while protecting the sensitive information within the original dataset. |

Though some fundamental practices remain the same, properly managing a set of data that a research team has collected themselves involves different considerations than managing a dataset that is being repurposed. Insofar as data management is necessary for establishing data provenance, managing data that was algorithmically generated involves different considerations than data that was not. These considerations are discussed in forthcoming modules.

## 2.4 Data Ownership

Here is a question sure to catalyze spirited conversation: *Who actually owns research data?*

The answer is not so simple and has serious implications for how data must be managed.

### What is ownership anyway?

Even if simplifying a complex concept like data  “ownership” down to something like “Having a high level of rights and responsibilities over a set of data, this is not actually an easy question to answer. For research data, such rights and responsibilities are very granular and often spread amongst multiple parties.

In general, at academic institutions, the institution itself typically asserts ownership over the scientific record (including the data) for any research project conducted at the institution, under the auspices of the institution, or with institutional resources. In this role, the institution is ultimately responsible for ensuring that research is conducted ethically, responsibly, and in-line with any applicable rules and regulations. Under certain circumstances, ownership data collected by institutionally affiliated researchers may also be claimed by study sponsors or other parties.

But researchers are not without their rights to the data they acquire or collect themselves.  Typically, Primary Investigators are granted a degree of stewardship over research data. When researchers leave an institution, they are typically able to bring copies of their research data with them or maintain access in some way. If a PI leaves for another institution, ownership may also be transferred to that institution (following the receipt of appropriate permissions).

All of which is to say “ownership” is perhaps not the right framework. For the most part, behavior related to research data is not so much dictated by who owns it, but by applicable policies, contracts, and regulations. 

Both outgoing data (data originated at one institution that is being shared with parties elsewhere) and incoming data (data originated elsewhere that is being shared with researchers at an institution) may be subject to a **data use agreement**, a contractual agreement that establishes the following:

1. Who is able to use a given dataset  
2. The permitted uses of the dataset,  
3. The responsibilities of the users of the dataset

### But what about copyright?

Here is where things get (more) complicated.

According to the U.S. Supreme court, facts are not copyrightable[^3]. An individual cannot copyright the fact that on October 5th, 2023 it was over 90 degrees fahrenheit in Palo Alto California. 

So far, so good?

Works of authorship (including databases) *are* copyrightable and there can be substantial room for disagreement in terms of where research data falls on this continuum.

For primary data, the issue of copyright typically arises at the point of sharing. As will be covered in a later section, many research data repositories ask authors to assign a license to any data that they upload. Some of the most common options are outlined in **Table 2.03** below.

In general, it is preferable to assign as permissive a license as possible to a shared dataset in order to facilitate its reuse. Giving and receiving credit for contributions in academic research is typically based (rightly or wrongly) on authorship and citations. Credit is typically not connected to ownership and copyright. All of which is to say, cite your sources and peruse the forthcoming chapter on Data Sharing, which covers all of this in more detail.

For secondary data, as with abiding with any other contract and regulation, it is imperative that a research team understand and follow through with the terms of the copyright license, the data use agreement, and any other terms that have been assigned to the data. There may be very specific provisions related to how the data should be managed, which will need to be integrated into the research workflow.

## 2.5. Taking CARE with data

Conversations about data management typically focus on the tools, methods, and behaviors that maximize the utility of data by academic researchers, scholarly institutions, and the broader scientific enterprise. Less emphasized is a nuanced understanding of historical context, power, and self determination.

This guide is almost certainly guilty of that as well. 

But any guidance on defining data and understanding ownership of data cannot conclude without a discussion of the broader contexts within which data is collected, used, and disseminated. 

One model for considering such issues is the CARE Principles for Indigenous Data Governance[^4]. These principles establish **data sovereignty** \- a group's (or individual’s) right to control and maintain their own data, including its collection, storage, and interpretation \- for indigenous communities across the world. 

The four CARE Principles are described in **Table 2.3**.

#### Table 2.3. The CARE Principles

| Principle | Description |
| :---- | :---- |
| **C**ollective Benefit | Data ecosystems shall be designed and function in ways that enable Indigenous Peoples to derive benefit from the data. |
| **A**uthority to Control | Indigenous Peoples’ rights and interests in Indigenous data must be recognised and their authority to control such data be empowered. Indigenous data governance enables Indigenous Peoples and governing bodies to determine how Indigenous Peoples, as well as Indigenous lands, territories, resources, knowledges and geographical indicators, are represented and identified within data |
| **R**esponsibility | Those working with Indigenous data have a responsibility to share how those data are used to support Indigenous Peoples’ self-determination and collective benefit. Accountability requires meaningful and openly available evidence of these efforts and the benefits accruing to Indigenous Peoples. |
| **E**thics | Indigenous Peoples’ rights and wellbeing should be the primary concern at all stages of the data life cycle and across the data ecosystem. |

While CARE was developed specifically as a response to the suppression and co-option of Indigenous knowledge, the principles also reflect the broad need to understand and address inequity within data ecosystems. 

This conversation is much bigger than can be covered in this guide and there is a great deal of excellent work on this topic, some of which is highlighted in the “Further Reading” section below. But, as researchers and teams conceptualize their data, where it comes from, and what it will be used for, it is vital that they take care.

## Definitions of Key Terms

**Data Sovereignty \-** A group's (or individual’s) right to control and maintain their own data, including its collection, storage, and interpretation 

**Data Use Agreement** \- A contractual agreement that establishes who is permitted to use and a dataset, the permitted uses of the dataset, as well as the responsibilities of the users of the dataset. The most typical consideration of a DUA is the protection of protected health data, but such agreements can be used in a variety of situations where the exchange of data is necessary.

**Metadata** \- Refers to information that facilitates the interpretation and/or use of research data. Can refer to formal metadata schemas (e.g. standardized ontologies) or to related documentation (data dictionaries, codebooks, protocols, etc). 

**Research Data** \- Broadly refers to the inputs or outputs required to evaluate, reproduce, or built upon the analyses or conclusions of a given research project. Throughout a research workflow, data may be categorized as “raw”, “intermediate”, or “final” products.

* **Primary Data** \- Data collected, processed, and analyzed by a research team to address specific research questions.  
* **Secondary Data** \-  Data collected for one purpose and subsequently repurposed, curated, and/or provisioned for another.  
* **Simulated Data** - Data synthesized through a stochastic process to augment or replace real-world data (i.e. to develop or improve artificial intelligence models, protect sensitive information, mitigate bias, etc).

**Research Workflow** \- The series of programmatic steps or practical ‘ways of doing things’ as data is collected, processed, and analyzed. Basically, where the research results came from.

## Further Reading

Borghi, J., & Van Gulick, A. (2022). Promoting Open Science Through Research Data Management. Harvard Data Science Review. [https://doi.org/10.1162/99608f92.9497f68e](https://doi.org/10.1162/99608f92.9497f68e)

Carroll, M. W. (2015). Sharing Research Data and Intellectual Property Law: A Primer. PLOS Biology, 13(8), e1002235. [https://doi.org/10.1371/journal.pbio.1002235](https://doi.org/10.1371/journal.pbio.1002235)

Carroll, S. R., Garba, I., Figueroa-Rodríguez, O. L., Holbrook, J., Lovett, R., Materechera, S., Parsons, M., Raseroka, K., Rodriguez-Lonebear, D., Rowe, R., Sara, R., Walker, J. D., Anderson, J., & Hudson, M. (2020). The CARE Principles for Indigenous Data Governance. *Data Science Journal*, *19*, 43\. [https://doi.org/10.5334/dsj-2020-043](https://doi.org/10.5334/dsj-2020-043)

Hummel, P., Braun, M., Tretter, M., & Dabrock, P. (2021). Data sovereignty: A review. *Big Data & Society*, *8*(1), 2053951720982012\. [https://doi.org/10.1177/2053951720982012](https://doi.org/10.1177/2053951720982012)

Miller, G., & Spiegel, E. (2025). Guidelines for Research Data Integrity (GRDI). *Scientific Data*, *12*(1), 95\. [https://doi.org/10.1038/s41597-024-04312-x](https://doi.org/10.1038/s41597-024-04312-x)  

## Footnotes

[^1]:  [Final NIH Policy for Data Management and Sharing](https://grants.nih.gov/grants/guide/notice-files/NOT-OD-21-013.html)

[^2]:  Data lifecycles are visualizations that illustrate different stages of data management and describe how data flows through a research project from start to finish. One such model is the Research Data Framework \- Hanisch, R. (2023). *NIST Research Data Framework (RDaF): Version 1.5* (NIST SP 1500-18r1; p. NIST SP 1500-18r1). National Institute of Standards and Technology. [https://doi.org/10.6028/NIST.SP.1500-18r1](https://doi.org/10.6028/NIST.SP.1500-18r1)

[^3]:  *Feist Publications, Incorporated v. Rural Telephone Service Company, Incorporated*
