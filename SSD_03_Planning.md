# Planning for Data Management

This chapter deals with the development of documentation describing how data is to be managed over the course of a project. This includes *data management and sharing plans* (DMSPs) as well as documentation designed for internal use, such as standard operating procedures.

This chapter is built on the principle that it takes planning to manage data well.

[Last Chapter - Defining Research Data](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_02_defining-data) | [Back to the Table of Contents](https://johnborghi.github.io/Supporting_Scientific_Data/) | Next Chapter (Coming Soon!)

---

|| **Key Points for this Chapter** |
| :---- | :---- |
| 1\. | Developing and documenting plans related to how data will be saved, organized, and described helps the research process proceed smoothly.  |
| 2\. | Data Management and Sharing Plans (DMSPs) are intended to communicate to research funders how data will be archived and made available to others. For NIH, the contents of these plans are written into the terms and conditions of the award.   |
| 3\. | Data-related standard operating procedures (SOPs) are more thorough descriptions of how data should be managed during the day-to-day course of research. These are created and implemented collaboratively by the research team. |
| 4\. | Plans should be updated as needed and revisited often. |


| | **Supplementary Materials for this Chapter** |
| :---- | :---- |
|[DMSP Rubric](https://zenodo.org/records/7710001)|A rubric for evaluating the contents of an NIH data management and sharing plan. This rubric is meant for educational purposes only and includes an annotated DMSP template. |
|[SOP Template](https://docs.google.com/document/d/1ATWE-zzJoMjR9dumo_e3fOROabIrvRct/edit?usp=sharing&ouid=118445803869398413021&rtpof=true&sd=true)| A template for writing a Standard Operating Procedure. The example given is a very important activity in the scientific research enterprise, making a decent cup of coffee.
|[Lab Manual Template](https://docs.google.com/document/d/1kPYt2Jo_eI18PlkoMMqAe0McgZC44cad1ErI8CJbF10/edit?usp=drive_link)| SOPs are not necessarily standalone documents. This template describes how to develop a lab manual.|

---

##3.1. Planning for Data Management

“If you fail to plan, you plan to fail”.

The above quote is, of course, a line from the song “Masterminds” by Taylor Swift. 

Ok, ok. The sentiment actually precedes the release of the album *Midnights* by at least a century. Often attributed, without sourcing, to Benjamin Franklin, this catchy aphorism first appeared in print in the early twentieth century.

Regardless of who said it and in what context, this sentiment also applies to managing scientific data. 

Data management begins **BEFORE** any scientific data is collected or acquired. It is, very occasionally, possible to go back and clean up a messy project workflow or dataset. But such efforts are neither particularly efficient nor recommended. Reconstructing your own work after the fact is a headache under the best of circumstances and a break in data provenance can have all sorts of consequences. More than one research effort has been delayed or doomed because of a lapse in data management.

The importance of documentation is the subject of another chapter. But a plan for data management is most effective when it has been properly documented and communicated. A “way of doing things” that is not written down can lead to confusion and ambiguity. A document that is never examined or revisited is just filling space in a filing cabinet or hard drive. 

**The Data Management Plan**

There is a bit of irony in the fact that the term “Data Management Plan” (DMP) does not have a standardized definition. Historically, it has been used to describe both relatively short documents that are submitted as part of grant and project proposals and also more thorough protocols that researchers maintain internally (such as standard operating procedures). Confusing matters further, is the increasingly common use of “Data Management and Sharing Plan” (DMSP) among funding agencies in the United States.

To minimize confusion, this guide will use the term **Data Management Plan** to describe *any* plan related to data management. The term will then be broken down as follows:

* **Data Management and Sharing Plans (DMSPs)** \- Plans written as part of grant or project proposals. These are typically relatively high level and the main users are program staff at research funding agencies, who need to evaluate compliance with related policies and regulations.  
* **Standard operating procedures (SOPs) \-** Plans that describe precisely how data should be managed during the day-to-day course of a research effort. These documents may or may not be standalone and the primary users are typically researchers working on a given research effort, who need to learn and implement the standardized practices described in the plan.

The goal of both of these categories is to establish standards or standardized practices that a research team will adhere to over the course of a research effort. This is not to say that a data management plan is immutable. Things change and quality improvement is a good thing. DMPs can be updated when needed, but the changes need to be recorded and communicated. 


## 3.2. Planning Ahead, Playing FAIR

The value of a data management plan is not just its contents, but in the practice of considering data-related activities ahead of time. There are some data-related practices that MUST be considered well in advance. For example, if you are planning to eventually share data that was acquired from human research participants, that fact typically must be written into consent-related documentation. But also, considering issues such as how data will be saved, where it will be saved, and (perhaps most importantly) who will be responsible for ensuring it is saved properly will save prevent a lot of headaches later on.

Putting together a data management plan is an important early step in a research project and necessitates thinking through your entire research workflow. 

Which is to say, start planning early and revisit your plans often. It may seem tedious in the moment, but your future self - returning to your data perhaps after doing a deep dive in the source of a Taylor Swift quote - will thank you for being so detail oriented.

Because decisions you make early effect what you can do with your data later, you need to carefully consider:

* What is your data?  
* What do you want to do with your data?  
* What can you do with your research data?  
* What can’t you do with your data?  
* What mandates, regulations, expectations, and guidance exist related to your data.  
* Who is responsible, and for what?

Answering these questions through the development and communication of a data management plan will help you and your collaborators stay organized and work together to ensure the usability of your data over time. A widely cited framework for understanding data management provides a good starting point \- FAIR.

The FAIR Guiding Principles[^2] (see **Table 3.1**) were originally developed to describe data-related infrastructure (e.g. data repositories). However, **FAIR** is now often used colloquially to refer to the degree to which individual practices, strategies, and tools facilitate the (re)usability of research data. Individual datasets can even be considered as existing along a continuum of FAIRness. FAIR does not imply that data is open or available for free, but rather that it is usable.

**Table 3.1 The Fair Guiding Principles**

| Principle | Description |
| :---- | :---- |
| **F**indable | Data should be easy to find by both humans and computers (e.g. use of standardized file names, persistent identifiers) |
| **A**ccessible | There is a clearly defined method for accessing the data (e.g. use of standardized file organization, data storage and backups). |
| **I**nteroperable | Data should be usable across a range of applications and workflows (e.g. use of standards, common file formats) |
| **R**eusable | Data should be saved, organized, and described with its future (re)use in mind, even if there are no plans to share it openly. |

Remember that data management is about ensuring the quality and usability of research data over time. FAIRness is a component of that, one that often needs to be addressed directly when working with research funding bodies and other data stakeholders. But the practice of data management is much broader than addressing FAIRness. For example, the FAIR guiding principles do not readily address sensitive and/or regulated data. FAIRness is an end-state for data, but data management is a continuous process.

## 3.3. Data Management and Sharing Plans

Over the last two decades, realizing the benefits of large-scale data sharing and reuse, research funding bodies such as the National Science Foundation, National Institutes of Health, and Patient Centered Outcomes Research Institute have begun to require the inclusion of **data management and sharing plans (DMSPs)** as part of project proposals.

Typically these documents are included as part of the initial submission of the proposal. While they generally do not factor into the evaluation of the scientific merit of the proposed work, funders may not disperse awarded funding unless an acceptable plan is in place. In some cases, such as for DMSPs created for NIH proposals, the content of a plan for a funded proposal becomes part of the terms and conditions of the award. 
  
A data management and sharing plan written for a grant or project proposal is typically a relatively short document (usually around two pages) that includes both a description of what data will be generated or acquired to fulfill the proposed work and outlines how that data will be preserved and made available to others.

However, different funders and even different institutes or directorates within the same funder may have different requirements for the contents of their plans. Often, specific requirements will be listed in the funding opportunity announcement, but below we have listed two additional sources of support for developing your data management and sharing plans. 

>**Tool Spotlight: [DMPTool](https://dmptool.org/)**  
>
>DMPTool is a free, web-based platform for developing and making the most out of data management and sharing plans. Researchers can use DMPTool to create data management and sharing plans in the format required by the National Institutes of Health and other funders. Uniquely, DMPtool also allows users to assign their plans a persistent identifier, which ensures they are easily connected to related datasets, publications, personnel, and other project elements. 
>
>[Access the DMPTool](https://dmptool.org/)  

Though some funders of biomedical research, such as the Patient Centered Outcomes Research Institute (PCORI), have had similar requirements for longer the Data Management and Sharing Policy instituted by the National Institutes of Health in 2023 catalyzed much of the current activity in biomedical research related to the development of data management and sharing plans.

This policy has two basic elements:

1. Submission of a Data Management and Sharing Plan for applicable proposals.  
2. Compliance with the awardee’s plan as approved by the NIH ICO.

In general, this policy applies to any proposal that will result in the generation of research data[^3]. Individual Institutes, centers, and calls for proposals may have additional recommendations or requirements but, as outlined in **Table 3.2**, all DMSPs submitted under this policy have six required elements:

**Table 3.2: Elements of an NIH DMSP**

| Element | Description |
| :---- | :---- |
| Data Type(s) | A description of data that will be managed and shared.  Not all data needs to be shared. Typically only the  “final” datasets underlying research conclusions are submitted to data repositories. However, all data \- throughout the entirety of the researh workflow \- should be well managed. |
| Related Tools, Software and/or Code | A description of any specialized software needed to use the data.  There is no explicit expectation in the DMS policy that custom software and/or code created as part of the analysis process be made available to others. |
| Standards | The standards and/or standardized practices that will be applied to ensure that shared data is usable and/or interoperable. If a formal standard does not exist for a particular type of data, practices related to addressing usability and interoperability should be addressed (e.g. documentation) |
| Data Preservation, Access, and Associated Timelines | How data will be stored over the long term and made available to others. The use of repositories is encouraged for both purposes, but they may not be appropriate under all circumstances. Often more data needs to be preserved (internally) than made accessible through a repository. Data should be made available at the time of publication or the end of the grant period, whichever comes first. Data should be made available for as long as researchers anticipate it being useful for the larger research community, institutions, and/or the broader public. |
| Access, Distribution, or Reuse Considerations | What, if any, limits there are on sharing (i.e., participant privacy). For some research projects, especially those that don’t involve work with data derived from human participants, there may be no such factors.  The DMS policy is not an open data mandate. Restrictions can be indicated as long as they can be justified. |
| Oversight of Data Management and Sharing | Who is responsible and for what? The primary investigator is ultimately responsible for developing, executing, and monitoring the activities and strategies described throughout the DMSP. Specific responsibilities can be delegated to others. |

Data management and sharing plans are supposed to reflect plans at the time they are written. If a change is needed over the course of the award, a prior approval request can be submitted to the corresponding NIH ICO[^4].

As of this writing, NIH DMSPs are generally evaluated by NIH program staff and this evaluation does not factor into peer review process or impact score. If changes are needed, they can be addressed during the just-in-time (JIT) period. However, when a project is funded, the contents of the DMSP become part of the terms and conditions of the award. Which underlines an important consideration when developing and updating a DMSP: **Only practices, strategies, and tools that are actually intended to be implemented should be included in a DMSP.**

(For the full effect, petend that last sentence is underlined instead of bolded, it is bolded for markdown and accessability reasons.)

> **Tool Highlight: [Data Management Rubric](https://zenodo.org/records/7710001)**
> 
> The NIH has not released the criteria program staff use to evaluate DMSPs. This does not mean that there are not rubrics and guidelines out there. But in the absence of other rubrics, here is one example that may be useful.
> 
> This rubric is, in no way, associated with NIH and was never intended as a means to provide quantitative assessment of DMPs. Instead, it should be used as an aid to understand what should be included in a DMSP.
> 
> If the rubric is a little overwhelming, similar guidance can also be found using this [annotated template](https://doi.org/10.5281/zenodo.10652155). Please use whichever is most useful to you.
> 
> [Access the rubric here.](https://zenodo.org/records/7710001)

## 3.4. Standard Operating Procedures (SOPs)

Here is a purely hypothetical situation:

>In a large, well-funded study, data is being collected by multiple researchers across multiple sites. Unfortunately, it is eventually discovered that not all the researchers were collecting data in the same way. 
>
>The primary investigators had developed an exemplary data management and sharing plan when applying for grants. But the researchers on the ground interpreted it in different ways. 
>
>As a result, much of the collected data is now effectively useless.

Just as a grant proposal outlines a research project from a relatively high level, a DMSP only provides an outline of how data is managed during the day-to-day course of a research project. A DMSP is an important starting point, but is not well suited for directing activity during the day-to-day course of a research project.

Over the course of a research project, there are instances in which a particular procedure needs to be done exactly the same way multiple times or by multiple people. A research group may have a "way of doing things", but to reduce miscommunication and increase efficiency, such procedures should be thoroughly documented and communicated as **standard operating procedures (SOPs).**

Within the context of Good Clinical Practice Guidelines, SOPs are detailed instructions meant to achieve uniformity in the performance of a specific function. This may sound very technical. But, in practical terms, a **standard operating procedure** is simply a document that contains instructions for completing a particular task the same way each time it needs to be completed.

**Developing a Standard Operating Procedure**

Because it is meant to be put into practice, developing a standard operating procedure should be an iterative and collaboratve process. Before it is disseminated, it should be tested and validated. Providing the research team with an SOP and then ensuring that they are all interpreting and implementing it in the same way would have gone a long way towards preventing the hypothetical situation described at the start of this section. An SOP is only useful if it is effectively communicated and put into practice.

SOPs should be formatted in a way that facilites their effective use. **Table 3.3** below provides an overview of what information should be included.

**Table 3.3. Information to be Included in an SOP**

| Section | Description |
| :---- | :---- |
| Purpose | The SOP should include a description of WHY is should be put into practice. This can be as simple as wanting (or needing) to standardize a set of processes.|
| Personnel | The SOP should include information about to whom it applies and who is responsible for ensuring that it is implemented properly. SOPs can apply to everyone within a research group, everyone within a broader collaboration, or whatever group makes sense given the activities described in the SOP.|
| Expectations| The SOP should include information about any expectations related to SOP. This may include the scope of the SOP (i.e. how broadly it should apply), the frequency by which it should be applied, etc|
| Step by Step Instructions| Finally! The SOP should include the step-by-step instructions for the activity in detail. The goal should be to leave as little room for alternative interpretations as possible.|
| Step by Step Instructions| Finally! The SOP should include the step-by-step instructions for the activity in detail. The goal should be to leave as little room for alternative interpretations as possible.|

> **Tool Highlight: [SOP Template](https://docs.google.com/document/d/1ATWE-zzJoMjR9dumo_e3fOROabIrvRct/edit?usp=sharing&ouid=118445803869398413021&rtpof=true&sd=true)**
> 
> Table 3.3. includes information that should be included in an SOP, but for a more practical example that can be adapted as needed, here is a template that includes perhaps the most important procedure in the scientific research enterprise- making a decent cup of coffee.
> 
> Why coffee? 
> 
> Mostly because of "cups". It turns out that the marks on the side of most coffee machines indicate "cups of coffee" rather than any standardized or widely accepted unit of measurement. Even the "cup" measurement widely used in food preperation varies depending on context. Here in the United States, a cup is custamarily 8 fluid ounces. Except when it isn't. A "legal" cup is 8.12 fluid ounces. A metric cup is about 8.45 fluid ounces and an "imperial" cup is about 9.61 fluid ounces.
> 
> All of which is to say, there is actually a lot of room for interpretation in most instructions for brewing a cup of coffee and that's before getting into issues like water temperature and grind.
>
> A good rule of thumb for any SOP is to document more than you think is necessary and in greater specificity than you think might be necessary. Do not assume that something that is clear to you will be clear to all.
> 
> [Here is the template.](https://docs.google.com/document/d/1ATWE-zzJoMjR9dumo_e3fOROabIrvRct/edit?usp=sharing&ouid=118445803869398413021&rtpof=true&sd=true)

An SOP can cover even the most “mundane” of activities, including setting standards for how project-related files should be named and organized. The SOP should reflect current practice, if a particular step needs to be changed for some reason, that should be reflected in the documentation and communicated to any team members affected.

SOPs are a resource. Training on them should be part of any onboarding process. They should be stored in a manner that is accessible to all team members, they should revisited regularly to ensure awareness among current personnel, and they should occasionally be audited to ensure they are being applied properly.

**Lab Manuals**

**Table 3.4.** provides an overview of the types of practices and details that can be covered in data management-related SOPs. This list of activities and expectations is not meant to be exhaustive or even applicable to all research settings. To the degree that it is possible, standardization of these types of practices within a research effort (and even between efforts) helps things proceed efficiently. That begins with having a plan.

**Table 3.4: Standard Operating Procedures**

| Element | Description |
| :---- | :---- |
| Onboarding procedures | A description of how new team members should become familiar with their responsibilities related to research data and any relevant data-related practices, strategies, and tools. Topics include: Data-related training that needs to be completed (e.g. HIPAA training, CITI training). Checklists and SOPs that need to be reviewed and implemented (see following sections). Gaining access to appropriate systems and tools (including secondary datasets, if applicable). Where to go for guidance and help. |
| Saving and backing up data | A description of how team members should save their data during the course of a project. Topics include: Where to find data and other materials How data should be saved. How data **should not** be saved (i.e. if data contains sensitive information). Where data should be backed up. The number and frequency of backups. |
| Data Organization | A description of how team members should organize data and other materials during the course of a project. Topics include: How to find data and other materials File naming conventions Directory/folder organization conventions Version control for “intermediate” forms of data (and other research products). |
| Documenting Data and Process | A description of how team members should maintain metadata, including documentation related to the content of data files, project procedures, contemporaneous notes, etc. Topics include: Where to find existing documentation. Expectations related to the use of tools (lab notebooks/ELNs, Protocols.io, etc) Conventions for maintaining data-level documentation (e.g. data dictionaries) Conventions for documenting research workflows (e.g. protocols, analysis pipelines, etc) |
| Data Archiving | A description of how team members should prepare data and other materials for long term storage. Topics include: How to access data and materials from completed and/or previously archived projects. What forms of data (e.g. “raw” vs. “final”) and related materials should be archived. Where archived data should be stored. |
| Data Sharing | A description of standard practices related to making data available to others. Topics include: How and where to access previously shared data. How to prepare data for sharing (e.g. de-identification procedures) Administrative procedures and checklists (e.g. DRAs, DUAs, etc) |
| Software and code | Topics include: Expectations related to the use of specific software tools and/or platforms. How and where to access custom code and scripts (if applicable). Standards related to version control |
| Roles and responsibilities | An outline of who is responsible and for what. Topics include: Expectations for all project members Specific responsibilities and who to contact. |
| Project closeout/Offboarding | A description of how team members should be offboarded from projects and practices related to project closeout. Topics include: Checklists and SOPs that need to be reviewed and implemented (see following sections). |

Given the exhaustive contents of Table 3.4., it is is worth pointing out that SOPs are not always standalone documents. Data management-related SOPs are often outlined as part of a **lab manual** or lab handbook, a document that covers a broad range of expectations and norms for a research group. 

Some example lab manuals that incorporate data management, include:

* The [Benjamin-Chung Lab](https://jadebc.github.io/lab-manual/) (Stanford University)  
* The [Fraser Lab](https://fraserlab.com/philosophy/) (UCSF)  
* [The Memory Modulation Lab](https://docs.google.com/document/d/1L1DhF3gKZKVGb_MDEmdqvBwm5thWiqyMy8AS_kzJnSM/edit) (Boston College)

> **Tool Highlight: [Lab Manual Template](https://docs.google.com/document/d/1kPYt2Jo_eI18PlkoMMqAe0McgZC44cad1ErI8CJbF10/edit?usp=drive_link)**  
> 
> Developing a lab manual provides an opportunity for a research group to carefully consider their philosophy, ethos, and culture. From a practical perspective, a lab manual also increases efficiency, as each member of the group understands what is expected of them and the lab’s “ways of doing things”. 
> 
> Much of the content in a lab manual is somewhat adjacent to what is in scope for a guide focused on data management but, because it overlaps with our focus on consistent and standardized practices, we have developed a template. 
> 
> This template should be viewed mostly as a starting point for groups who are interested in developing their own manuals. Different groups will have different needs for a document like this, so please feel free to adapt the parts that work for you and your group and pass over the parts that do not.
> 
> [Access the template here](https://docs.google.com/document/d/1kPYt2Jo_eI18PlkoMMqAe0McgZC44cad1ErI8CJbF10/edit?usp=drive_link)

## 3.5. Updating and Communicating Your Plans

Researchers plan and science laughs[^5].

A consistent feature of the research process is that things sometimes just don’t go according to plan. This is also the case for data management. Your data management plans should establish standardized practices, but this does not mean that they should be static documents. Similarly, any data management plan is only as useful as the degree to which it has been communicated to project team members.

**Updating and Communicating Data Management and Sharing Plans**

A DMSP is meant to reflect plans related to data management at the time it is written. SInce DMSPs are typically written for grant proposals, they are generally drafted before the processes of data acquisition and analysis have begun in earnest. Between the writing of the plan and implementation, a lot can change. 

NIH data management and sharing plans are expected to be updated over time. Changes must be requested and approved beforehand via the [Prior Approval Module](https://www.era.nih.gov/erahelp/Commons/Commons/Prior_Approval%20Module/OtherRequest.htm). Investigators must select “Prior Approval – Other Request”.

**Updating and Communicating Data-Related SOPs**

Data-related SOPs should be revisited frequently and updated as needed. Data SOPs should be stored somewhere where they can be easily found by project team members, should be included in onboarding procedures, and should be addressed regularly at team meetings.

## Definitions

**Data Management Plan** \- Documentation that describes data management and sharing-related practices and strategies. These include both data management and sharing plans written for grant and project proposals as well as more thorough documentation that describes standardized practices to be implemented during the day-to-day course of a research effort. This later category may include standalone documents or be included in broader materials (e.g. lab manuals).

**Data Management and Sharing Plan** \- A form of data management plan developed and submitted as part of a grant proposal. Typically data management and sharing plans are relatively short documents (two or so pages) with required elements, including a description of the research data that will be acquired or generated by the proposed work as well as how that data will be preserved and made available to others.

**FAIR Guiding Principles \-** A set of guiding principles initially developed to describe the desired characteristics of data-related infrastructure to facilitate the discovery and re-use of data assets by computational tools (i.e. machine readability). The term has now come to be used generally to refer to datasets that are not only available, but available in a *usable* form.

* **Findable \-** The dataset should be discoverable.  
* **Accessible \-** There should be a clear path for accessing the data.  
* **Interoperable \-** The dataset should be available in a form that enables it to be combined with like data and used by computational tools.  
* **Reusable \-** The data should be well described (i.e. rich metadata) with detailed provenance.

**Lab Manual \-** A set of documentation that lays out the expectations, standard operating procedures, and the details of a lab’s culture and philosophy. A lab manual may include standard operating procedures related to data management and sharing or may link to such SOPs stored elsewhere.

**Standard Operating Procedures \-** A set of step by step instructions for properly completing a routine activity. SOPs are an integral part of standardizing practices within a research team.

## Further Reading

Aly, M. (2018). The key to a happy lab life is in the manual. *Nature*, *561*(7721), 7–7. [https://doi.org/10.1038/d41586-018-06167-w](https://doi.org/10.1038/d41586-018-06167-w)

Dempsey, W., Foster, I., Fraser, S., & Kesselman, C. (2022). Sharing Begins at Home. *Harvard Data Science Review*, *4*(3), 10.1162/99608f92.44d21b86. [https://doi.org/10.1162/99608f92.44d21b86](https://doi.org/10.1162/99608f92.44d21b86)

Gonzales, S., Carson, M. B., & Holmes, K. (2022). Ten simple rules for maximizing the recommendations of the NIH data management and sharing plan. *PLOS Computational Biology*, *18*(8), e1010397. [https://doi.org/10.1371/journal.pcbi.1010397](https://doi.org/10.1371/journal.pcbi.1010397)

Hollmann, S., Frohme, M., Endrullat, C., Kremer, A., D’Elia, D., Regierer, B., Nechyporenko, A., & on behalf of Cost Action CA15110. (2020). Ten simple rules on how to write a standard operating procedure. *PLOS Computational Biology, 16*(9), e1008095. [https://doi.org/10.1371/journal.pcbi.1008095](https://doi.org/10.1371/journal.pcbi.1008095)


Tendler, B. C., Welland, M., Miller, K. L., & The WIN Handbook Team. (2023). Why every lab needs a handbook. *eLife*, *12*, e88853. [https://doi.org/10.7554/eLife.88853](https://doi.org/10.7554/eLife.88853)

Wilkinson, M. D., Dumontier, M., Aalbersberg, Ij. J., Appleton, G., Axton, M., Baak, A., Blomberg, N., Boiten, J.-W., da Silva Santos, L. B., Bourne, P. E., Bouwman, J., Brookes, A. J., Clark, T., Crosas, M., Dillo, I., Dumon, O., Edmunds, S., Evelo, C. T., Finkers, R., … Mons, B. (2016). The FAIR Guiding Principles for scientific data management and stewardship. *Scientific Data*, *3*(1), Article 1\. [https://doi.org/10.1038/sdata.2016.18](https://doi.org/10.1038/sdata.2016.18)

**For more on the NIH Data Management and Sharing Policy**

* [FINAL NIH Policy for Data Management and Sharing Policy](https://grants.nih.gov/grants/guide/notice-files/NOT-OD-21-013.html)   
* [Sharing.NIH.gov \- Guidance on data management and sharing from NIH](https://sharing.nih.gov/)

[^1]:  Smale, N. A., Unsworth, K., Denyer, G., Magatova, E., & Barr, D. (2020). A Review of the History, Advocacy and Efficacy of Data Management Plans. *International Journal of Digital Curation*, *15*(1), 30\. [https://doi.org/10.2218/ijdc.v15i1.525](https://doi.org/10.2218/ijdc.v15i1.525)

[^2]:  Wilkinson, M. D., Dumontier, M., Aalbersberg, Ij. J., Appleton, G., Axton, M., Baak, A., Blomberg, N., Boiten, J.-W., Da Silva Santos, L. B., Bourne, P. E., Bouwman, J., Brookes, A. J., Clark, T., Crosas, M., Dillo, I., Dumon, O., Edmunds, S., Evelo, C. T., Finkers, R., … Mons, B. (2016). The FAIR Guiding Principles for scientific data management and stewardship. *Scientific Data*, *3*(1), 160018\. [https://doi.org/10.1038/sdata.2016.18](https://doi.org/10.1038/sdata.2016.18)

[^3]:  For a list of activity codes that fall under under the NIH Data Management Policy \- https://sharing.nih.gov/sites/default/files/flmngr/List-of-Activity-Codes-Applicable-to-DMS-Policy.pdf

[^4]:  https://grants.nih.gov/grants/guide/notice-files/NOT-OD-23-185.html

[^5]:  Alternatively, and with apologies to Robert Burns, “The best laid plans of (lab) mice and (research)men(tors) often go astray.”
