# Sharing Data 

| [Last Chapter - Saving and Organization](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_05_saving-organizing) | [Back to the Table of Contents](https://johnborghi.github.io/Supporting_Scientific_Data/) | Next Chapter - Coming soon! |

## Chapter Summary

This chapter covers how researchers can share data effectively and appropriately with themselves, their collaborators, and more broadly.

The chapter is built around the principle that all data must be managed, but not all data necessarily needs to be shared (openly).

| [Principles of Good Data Management Practice](https://johnborghi.github.io/Supporting_Scientific_Data/supplements/SSD_good-dm-practice) | ["Good Enough" Practices in Data Management](https://johnborghi.github.io/Supporting_Scientific_Data/supplements/SSD_good-enough) |

|  | Key points for this chapter |
| :---- | :---- |
| 1\. | Data sharing is the release of data for use by others. This encompasses both sharing for collaborative purposes (e.g. sharing with labmates or collaborators) and sharing more broadly for the purpose of facilitating reuse. |
| 2\. | Some research data can be shared without restrictions. But a good rule of thumb is to share “as openly as possible, as closed as necessary”|
| 3\. | In general, when sharing data for reuse purposes, sharing should occur via established data repositories. If this is not possible, it is important to clearly communicate what mechanisms (if any) can be used to access the data. |
| 4\. | If specialized repositories are not available for the type(s) of data you want to share, multiple “generalized” data repository solutions are available. |
| 5\. | Any data that is shared should be shared in a usable form. |

|  | Supplementary materials for this chapter |
| :---- | :---- |
| [Data Index Checklist](https://docs.google.com/document/d/1qTkKoNBriP5bqoJWyvZl29xvjue9WJIRgCnW7ZQP3LY/edit?tab=t.0) | This document provides guidance to research teams who need to keep a record of how and where their research data is saved. |

## 6.1. Sharing with yourself and others

It may be a little strange to consider it in these terms now, but the advent of scientific journals substantially increased the accessibility of scientific research. 

This did not always look like science communication as we understand it today, of course. Almost everyone who has taken high school biology has the phrase “the mitochondria is the powerhouse of the cell” burned into their memory. This idea was first postulated at the turn of the 20th century by Benjamin F. Kingsbury \- the great great grandfather of this chapter’s author \- in an almost incomprehensibly dense article[^1]. 

But still, the advent of the scientific journal was a watershed moment in the dissemination of science. No longer were research findings communicated only through personal correspondence or research society meetings. Any researcher with a subscription to the journal and sufficient expertise could stay up-to-date with the latest research in their field. This change came from technological development \- namely, the invention of the printing press. 

Another technological development, the internet, has helped researchers disseminate their findings even further. Open Access[^2] is a set of practices through which research outputs are disseminated freely online. Though often discussed in financial terms, open access has multiple dimensions related to the rights of both authors and readers to post and make use of an article’s content. A given paper may, colloquially, be said to be “open” but it is more accurate to say that it exists along a continuum of “openness”.

The internet has not only made sharing scientific findings easier, it has also significantly eased the process of directly sharing the evidence that underlies those findings. Kingsbury’s proposal that mitochondria plays a role in cellular respiration was based mostly on morphological observations. His paper lacked the figures or materials that would be commonly included in a modern research paper to strengthen his point. But fast forward more than a century and it is now very common for data, code, and other materials to be shared alongside a research paper.

Central to both this guide and the Good Data Management Practice more generally is understanding that science is a process. Historically, the communication of science has focused on the communication of findings or results. Benjamin Kingsbury did not communicate every single step of his experimental protocols or share the images that underlied his theories about mitochondria. But how could he? The technology to even capture his data in a way that could be reliably shared did not exist until the invention of the electron microscope and the first high resolution photos of mitochondria weren’t published until the 1950s[^3].

But researchers today have far more tools at their disposal to share not just their conclusions but also the processes that gave rise to those conclusions.

**Data sharing** \- which can be broadly defined as making data available for use by others \- can be thought of as continuous with data management. Many of the same considerations and motivations apply. In fact, managing data as if it were going to be shared with another researcher can be a helpful shorthand when considering related practices and strategies. 

This chapter is unapologetically pro-data sharing, if for no other reason than it aligns with the notion that science is a process not a result. But Good Data Management Practice does not necessarily require that all data be shared broadly. Not all data is useful to share broadly and there are often very good reasons why the sharing of certain forms of data or data related to certain topics needs to be carefully controlled.

> A Note on Planning
>
> Planning is discussed [elsewhere in this guide](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_03_Planning) as a vital element of Good Data Management Practice, and nowhere is that more true than data sharing.
>
> From a purely practical standpoint, the process of sharing data is most efficient when it has been planned for in advance. It is not (always) impossible to curate a dataset so that it can be effectively shared after the fact, but it is (usually) quite the headache. While there may be some real startup costs to developing a robust system for data management, good day-to-day data management makes it far easier for shared in a usable form whenever a researcher needs with whomever a researcher needs.
>
> But not every difficulty in data sharing comes down to practicality. Especially when dealing with data from human research participants, some data absolutely needs to be protected from unauthorized access. The safety, privacy, confidentiality of partificants must be ensured. And consenting to participate in a research study is very different than consenting to have your data shared with the world.
>
> It is one thing for a research team to store personally identifiable information about their participants on an encrypted system. It is quite another to share that information with others.
>
> A future chapter will focus specifically on sensitive data. But, while there are ways to share information that once sensitive or enable participants to give their informed consent for data to be shared, *data sharing must be planned for in advance*.

When considering related practices and strategies, it can be useful to describe data sharing based on purpose:

* **Sharing for collaboration** \- The sharing of research data *within* the confines of a given research effort. Typically, this involves one researcher (or team) sharing data amongst themselves and with their collaborators (e.g. statisticians, other research professionals).  
* **Sharing for reuse** \- The sharing of research data *beyond* the confines of a given research effort. Most often, this refers to sharing with individuals who were not involved in the data’s acquisition, transformation, analysis, or initial publication.

Of course, researchers don’t just share data, they also make extensive use of shared data. So it can also be useful to describe data sharing based on direction:

* **Incoming Data** \- Data that has been acquired or received from an external source (i.e. from parties outside of a researcher’s institution).   
* **Outgoing Data** \- Data that is being shared with an external source (i.e. with parties outside of a researcher’s institution).

In practice, these distinctions can be a little blurry. A researcher may share data with a collaborator for them to reuse. A research effort may involve acquiring original data and combining it with datasets from a variety of outside sources. Every possible situation is probably occuring at the nearest research institution. But, before sharing any data or working with any shared data, it is important to know the answer to three very important questions (see **Table 6.1**).

**Table 6.1. Three questions about data sharing**

| Question | For sharing data | For using shared data |
| :---- | :---- | :---- |
| What can you do? | Are there any ethical concerns, regulations, contractual terms, or other reasons why data sharing needs to be restricted or constrained? | Are there any ethical concerns, regulations, contractual terms, or other reasons why the use and dissemination of already shared data needs to be restricted? |
| What do you need to do? | Are you subject to expectations or policies that require you to control access to the data, restrict use of the data, or share (or not share) the data (i.e. those meant to protect participant privacy).  | Do you need to abide by expectations or policies that require you to control access to the data, restrict use of the data, or share (or not share) the data (i.e. those set by copyright terms, data use agreements, etc). |
| What do you want to do? | With your answers to the first two questions in mind, are there data sharing-related activities that you would like to pursue (i.e. to foster openness, reproducibility, etc) that exceed what is strictly required?  | With your answers to the first two questions in mind, are what uses of shared data would you like to pursue?  |

## 6.2. Sharing and Not Sharing

The chapter on [Understanding Data Management](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_01_introduction) outlines the motivations for engaging in Good Data Management Practice. Many of those same motivations apply to data sharing. But sharing data is only worthwhile if the data is actually (re)usable. This chapter will circle back to and expand upon these but, when considering if data has been shared effectively, researchers should themselves:

1. Is there a clear path for accessing the shared data?
2. Is the data shared in a form or format that would allow it to be used by others?**
3. Is the data sufficiently well described to allow it to be used by others?
4. Are the links between the data and any related materials (or versions) defined?
5. Is the data shared in a manner that allows credit for its use to be given and received?

But, before delving deeper into the nuts and bolts of releasing data to others, here are some common objections to data sharing.

### Why not share with others?

Some of the most common objections to data sharing are discussed in **Table 6.2.** below. Responding to these objections is not intended as a criticism for any researcher who may raise them. The widespread sharing of data for the purposes of reuse is a relatively new expectation in many areas of science. Related practices and tools can feel like (and often are) an added burden for already overburdened research teams. Related policies and requirements can be confusing, even for data sharing experts and advocates and experts. And for researchers, the push to share data broadly may or may not necessarily align with professional incentives that mostly emphasize the publication of journal articles.

**Table 6.2: Common Objections to Sharing Data**

| Objection | Response |
| :---- | :---- |
| **Concerns about being scooped:** Sharing data may result in another party publishing one of your findings before you can. | Though this is a widespread and understandable concern, there is very little evidence that it actually occurs- especially following the sharing of research data. |
| **Concerns about misapplication:** Sharing data may result in its (intentional or unintentional) misuse by another party. | Especially for research that touches on sensitive issues (politically, socially, etc), this is very understandable. Combatting disinformation and misinformation is beyond the  |
| **Concerns about research parasitism:** Sharing data may result in another party using it without giving appropriate credit. | Though such norms are best established for publications, it would be bad academic practice to use a shared dataset without proper attribution (at least a citation). |
| **Concerns about maintaining participant privacy**| Data sharing does not necessarily require sharing data openly. It is often possible to share sensitive following a de-identification process or via a mechanism that controls access. Even if the data itself cannot be easily shared in any form, it is generally possible to share metadata. |
| **Concerns about the time, resources, and expertise needed to share properly** Sharing data properly does come with a cost, even if is just researcher time. |  Hopefully this guide has been helped to make your research workflow such that you are more prepared to share data. Sharing does also require resources. From a financial perspective, deposit fees can often be paid through grants or are subsidized by the institution. As for the expertise, Stanford has data management and sharing experts who are ready to help. Their contact info is at the end of this section. |

### Why share with others?

Stanford seismologist and champion of “really reproducible” research Jon Clærbout emphasized the importance of sharing the data and code underlying research findings[^4]. His views were later distilled by Jonathon Buckheit and David Donoho (also from Stanford) into the following slogan (emphasis from the original)[^5]:

*“An article about computational science in a scientific publication is not the scholarship itself, it is merely **advertising** of the scholarship. The actual scholarship is the complete software development environment and the complete set of instructions which generated the figures.”*

This is not substantially different from the definition of research data expounded upon in this guide, as encompassing all of the information and materials needed to trace a research workflow. Though publications are still the major currency within the incentive structure of science, there is a tremendous amount of scholarship in in the data, code, and other materials that underlie the findings discussed in the paper. These objects are not a precursor to the research, they are the research.

So, from one perspective, a major motivation for sharing data is the same as the major motivation for publishing papers \- to communicate research. The internet and the subsequent development of data repositories and other platforms provides an opportunity to do that in ways that were not feasible until relatively recently. If anything, being able to establish data provenance through careful management and sharing is even more relevant in the age of large language models.

The other major motivation for sharing research data is to facilitate its reuse. Sharing does not just allow the original research team to better illustrate the path they took from research idea to dataset to research results, it allows others to explore other paths. Some of the earliest calls for research data to be shared broadly were motivated by work attempting to synthesize or look across large bodies of knowledge[^6]. Science is not just a process, it is a highly collaborative process. Sharing data helps to maximize that charactor.

Of course, this does not mean that all data can be shared in the same way.

### The Dimensions of Data Sharing

At first blush, making data available for use by others might seem like a relatively straightforward proposition. Most researchers have some degree of experience looking over a dataset with a colleague or sending data to collaborators via e-mail or cloud storage. But effectively and appropriately sharing data requires navigating a number of considerations about what data should be shared, with whom, and for what purpose.

Like many things in science, data sharing is a continuum. **Table 6.3.** below lays out some of the different dimensions of data sharing from restricted (essentially not shared beyond the original research team) to unrestricted (made available for unrestricted reuse). The middle “controlled” column encompasses the broad and varied set of circumstances that arise when there are limits to the degree to which data can be shared. 

This organization is not meant to be prescriptive, there are very important reasons why the sharing of certain types of data needs to be carefully controlled. 

**Table 6.3. Dimensions of Data Sharing**

|  Dimension | Restricted | Controlled | Unrestricted  |
| :---- | :---- | :---- | :---- |
| **Completeness of shared data:**   *What* form of the data (if any) will be shared with others. | The data itself will not be shared, but metadata and other materials may be discoverable (i.e. through a data catalog). | Only certain forms of the data (e.g. processed data, aggregated data) or will be made available. | Every element needed to reproduce the research workflow is shared. |
| **Breadth of sharing:**   *Who* the data is to be shared with. | Data will only be made available to (select) members of the research team. | Access to data will be controlled (i.e. users may need to verify their identity, their qualifications for handling the data, the appropriateness of the proposed use, etc) | Data will be made easily discoverable and available through a repository that is open to the public. |
| **Time of sharing:**   *When* data will be made available for use by others.  | Data will not be shared at any point in time. | The data will be released for use by others after an identified embargo period. | Data will be made available immediately. |
| **Use of shared data:**   *How* the shared data can be used by others. | (Re)use of the data will not be permitted. | The allowed uses of shared data will be articulated, such as through a data use agreement | Data will be shared under terms that allow for unrestricted (re)use. |

Note that this table does not address the issue of “how” data should be shared. This is addressed below, but also depends on a whole host of factors- including applicable policies and expectations, the type(s) and content(s) of data being shared, logistical concerns (i.e. the size of the data), and the development of infrastructure.

## 6.3 What to share (and what not to share)

As we previously discussed, all of the information and materials needed to reconstruct a research workflow can be considered as scientific data. In practice, this can include quite a large number of files, documents, and other materials. The good news is that, while all of this needs to be managed, (probably) not all of it needs to be shared.

The characteristics of a set of data will also substantially affect how and with whom it can be shared. For example, in general, it is more straightforward to share de-identified data than data containing personally identifying information. For more on this, 

When approaching the question of *what* in the context of data sharing, consider what recipients will need and expect from the data. Or conversely, what would *you* need and expect from shared data.

### What to share for collaboration

The forms of data that should be shared for the purposes of collaboration will depend on the characteristics of the data and the needs of the collaborative work. This is, admittedly, not particularly specific or helpful guidance. But some additional insight can be gleaned from expectations for authorship.

For example, the International Committee of Medical Journal Editors (ICMJE) states[^7] that authors on scholarly works should:

*“...Be accountable for all aspects of the work in ensuring that questions related to the accuracy or integrity of any part of the work are appropriately investigated and resolved.”*

In practice, this means anyone listed as an author on a scholarly work should \- at the very least \- be able to locate and navigate through the related data during and following the research process. As covered in the chapter on [Defining Research Data](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_02_defining-data), scientific data takes many forms over time, including: 

* The raw data  
* Intermediate forms of the data  
* Metadata and documentation about the data, changes made to the data, and decisions made along the way.  
* “Final” versions of the data (i.e. those that underlie research findings)  
* Any other related materials (e.g. custom code).

Ensuring that members of a collaborative research team have access to data DOES NOT necessarily mean that everyone should have the ability to edit or change all of these materials at any time. Even when sharing for collaboration, there are occasions when data sharing must be limited. The issues outlined in **Table 6.4**. Are typically discussed in terms of sharing for re-use, but also apply in the context of sharing with more immediate collaborators.

### What to share for reuse

It depends. 

A good rule of thumb when considering what data and materials to share for reuse (i.e. the data that is made available to those outside a research group) is to work towards being “as open as possible, but as closed as necessary[^8]”.

In practice this means sharing what would be the most useful for other researchers while also being vigilant in respecting factors that limit the degree to which data can be shared. Some of these factors are outlined in **Table 6.4**.

Some forms of data simply cannot be shared in a usable form. In such cases, it may be most appropriate to consider sharing in a more *constrained* fashion. 

**Table 6.4. Limitations on sharing data**

| Reason for limit | Description | Steps researchers can (potentially) take |
| :---- | :---- | :---- |
| Potential to compromise participant privacy or confidentiality  | Datasets that contain identifying information for human participants pose a risk for their privacy and confidentiality. | Participant privacy and confidentiality must be centered in all data management and sharing-related activities. Sharing identifiable information within a research collaboration necessitates the use of secure research environments and/or processes that remove or mask identifiable information (e.g. deidentification).  Sharing for reuse requires deidentification. For some types of data or for data containing certain information, deidentification may not be possible or would result in a dataset that is not useful. Under these circumstances, data can not be shared.Consider sharing other materials and information as appropriate.  |
| Informed consent does not allow for sharing | Templates for informed consent documentation (e.g. consent forms) often includes language stating that data will not be shared broadly. Different institutions interpret this language differently, but such statements typically are seen as limiting sharing data for reuse. | The informed consent of research participants must be respected. Typically this language does not limit the sharing of data within a research collaboration. But if a consent document explicitly states that data will not be shared more broadly, then it cannot be shared more broadly. Work with the IRB to include appropriate language about sharing into your consent documentation moving forward. |
| Restrictions imposed (or anticipated) from research-related agreements | If you are making use of secondary data as part of your work or your work may eventually have intellectual property implications (e.g. a patent), then you will likely be limited in terms of what materials you can make available.  | Limits imposed by data use agreements and other contracts need to be respected.  Consider sharing other materials and information as appropriate (e.g. the workflows, codes, etc that someone with access to your data would need to build upon your research results). |
| Restrictions based on federal, state, local, or Tribal law, regulation, or policy. | A constellation of policies and regulations limit the degree to which certain forms of data can be shared. This includes the Health Insurance Portability and Accountability Act (HIPAA), but also the laws and regulations of the locales and communities where data is collected and stored. | Adherence to applicable laws, regulations, and policies must be maintained.  |
| Practicality  | There is not currently the infrastructure to efficiently share some types of research data. The data may be too large or in a format that is practically difficult to share (e.g. non-digital data). | The ecosystem for sharing research data is rapidly evolving. Datasets once thought to be too large to share are now shared as a matter of course. If your data is too large to share, ensure that it is properly saved and backed up. Sharing may be possible in the future. Also consider sharing a sample or subset of your data. |

## 6.4. When and with whom to share

When sharing data for collaboration, the timeline will depend on the research workflow. In general, timeliness will help a research proceed efficiently and effectively. To ensure that data can be shared efficiently, it should be kept well organized. For more details, see the chapter on Data Storage and Organization.

If you sharing for reuse, the most common and useful time point for releasing the data is upon the publication of any related research findings. Sharing upon publication can take a bit of planning.  We recommend beginning the process of sharing data well before any related papers are published. If possible, data should be ready for sharing *upon submission.* Again, a way to ensure that this process is efficient is to ensure that data is stored and organized well ahead of time. 

“As open as possible, but as closed as necessary”.

In this context, *openly* refers to making data and other research materials broadly accessible \- easy to find, easy to use, and easy to build upon. When sharing for collaborative purposes, this involves implementing many of the practices we have discussed previously. Everyone on the research team who needs to have access should have access. 

In terms of sharing beyond the immediate research team, we have often encountered biomedical researchers who believe that they are unable to share their data because doing so would compromise the privacy of their participants. This is a highly laudable position. But even in biomedical research, it is often the case that controlled forms of data sharing are possible.

**Controlled access** is an umbrella term that covers a variety of activities and mechanisms that set certain conditions on who has access to shared data and for what purpose. Common forms of access control include asking researchers who want to make use of shared data to verify their identity, their qualifications for properly handling the data, and/or the appropriateness of their proposed research. 

There are a variety of mechanisms for controlling access to data. **Data use agreements** (DUAs) are contracts between the individual or organization that owns access to a data source and another individual or organization who wants to use the data for something. DUAs often place limits on who is able to access the data and the purposes for which it can be used. 

Some data repositories, such as the NIMH Data Archive, have “restricted access” features, meaning that data will only be shared under conditions set by the depositor and the repository. These conditions can include a formal application and approval process, IRB approval, or signing onto data use agreements. These types of access control are used for data in which there could be harm if the data were shared openly, there are limitations on usage within the consent, or certain indirect identifiers must remain in order for the data to remain usable for analysis.

## 6.5. How to share data

A common way of sharing data for the purposes of collaboration is by sending files back and forth; through e-mail, or slack, or any of the other innumerable tools used by researchers in the 21st century. This is not necessarily problematic in every circumstance but, especially as the number of collaborators grows, access problems and version-related confusion can become major issues.  As an e-mail conversation grows in length, it can become more difficult to track who is accessing the data and what changes are being made between different versions. To minimize these kinds of issues, it is often preferable to share data for collaborative purposes through platforms and tools that allow for some form of managed access and version tracking.

### How to share for reuse

Considering the multifarious nature of scientific data and the constellation of factors that affect how, where, and with whom it can be made accessible, it is not surprising that there are a number of different mechanisms through which data can be shared.

Some of the most common ways of sharing data are described in **Table 6.5.**

**Table 6.5. Mechanisms for Sharing Data**

| Mechanism | Description |
| :---- | :---- |
| “By Request” | Access to the data is provided by the corresponding author of any associated manuscripts. This mechanism is simple to describe, but logistically difficult in practice.  The requestor must have the author’s current contact information (which may or may not be listed in the article) and the author must continuously have the data on hand to respond efficiently to requests.  We do not recommend this approach under most circumstances. But, particularly if some degree of access control is required, it can work if there are established processes in place for requesting, sending, and receiving the data.  |
| Through a working storage system  | Access to the data is provided via a link to a to Google Drive, Box, Github, or an equivalent system. This is relatively simple for groups who are already working with these systems to share data for collaborative purposes. Unfortunately, these systems typically lack two features that are needed to ensure the viability of longer-term sharing: discoverability and persistence.  There is often no way to search these systems broadly to find data and there is no guarantee that the data will be discoverable or even preserved over time.  We do not recommend this approach. Data and other materials stored on these systems can often be easily and/or automatically preserved through other means. |
| Through a lab or departmental website. | The data is made available through a lab website (e.g. a link to a lab server). Again the issues here are discoverability and persistence. We do not recommend this approach unless there is no other way of making the data available. |
| As a supplementary material to a published paper | The data is submitted as a supplementary material for any related publications.  Scholarly publications often have strict rules about how the content of articles should be preserved and how information about different versions (i.e. updates, corrections) should be communicated. Unfortunately, the same is not always true for supplementary materials. This approach is often recommended by funders and publishers, but unfortunately platforms used to handle the publication process do not necessarily handle data well. |
| Through a data repository | A **data repository** is a platform that facilitates the preservation, organization, and discovery of research data.  Whenever possible, we recommend sharing data through the appropriate data repository. |

The functions of a **data repository** are outlined in **Table 6.6.** below. As is evident from this extended definition, the term “repository” can be used in slightly different ways in the context of data management and sharing. For example, a Github repository is like a data repository insofar as it is a place where files, code, and other materials can be uploaded and shared with others. But, while the contents of a Github repository can change over time, a key aspect of a data repository is that its contents are typically meant to be persistent and easily discoverable over time. 

**Table 6.6. Major functions of a data repository**

| Function | Description |
| :---- | :---- |
| Facilitates discoverability of data | A data repository helps users locate deposited datasets. This is often through the provision of persistent identifiers (DOIs, etc), but many repositories also provide metadata to facilitate searching and even search engine indexing. Complimentary tool: Data catalogs |
| Provides access to data | A data repository provides potential users with a path to acquiring the data, such as direct downloads, the use of APIs, or access to a secure environment. Acquisition of the user may involve agreeing to certain terms and conditions (e.g. licenses). Alternative tools: Data Use Agreements, Data Access Committees. |
| Stores and preserves data | A data repository archives deposited data in a fashion that renders it usable at present and also years (or even decades) in the future. This occurs through replication (backups), migration, and processes that ensure integrity/fixity. Some repositories even provide emulation. Alternative/complementary tool: Working storage systems, archival storage |
| Sets standards and curates data | A data repository provides formal or informal rules for keeping data organized and well described so that it can be used. This may involve using community metadata standards or setting *de facto* standards. Alternative/complementary tool: Data policies, DMSPs, data SOPs, etc. |

Among the advantages of sharing data through a data repository is that the repository handles the difficult job of ensuring that the data can be found. In practice, that typically means issuing an identifier for the data that can be included in journal articles.

Many data repositories issue **persistent identifiers (PIDs)** to deposited data. This term is used in slightly different ways throughout the data sharing community, but a PID can be generally understood as a digital identifier that permanently and unambiguously identifies a digital object or an individual. 

For American readers of this guide, think of a PID as a dataset’s social security number. The most common PID for data is probably the digital object identifier or DOI, but there are a whole family of data-related identifiers including ARKs and PURLs.

Other repositories issue ***accession numbers*** to deposited data \- unique identifiers that are assigned to a record or item in an archive. For most purposes, an accession number is mostly interchangeable with a PID. But an accession number may or may not have some of the more technical characteristics of a PID (see below).

> ### PIDapalooza
> 
> The United States Office of Science and Technology Policy (OSTP) defines a persistent identifier as *A digital identifier that is globally unique, persistent, machine-resolvable and processable, and has an associated metadata schema*.
>
> Persistent identifiers can be used for more than just data and articles of course.
> * There are PIDs for organization, such as the [Research Organization Registry (ROR)](https://ror.org/).
> * There are PIDs for tools, equipment, and resources, such as [Research Resource Identifiers (RRIDs)](https://www.rrids.org/)
> * There are even PIDs for people, like [Open Researcher and Contributor IDs (ORCIDs)](https://orcid.org/).
>
> All of these help with problems related to disambiguating one object from another. This is useful when less consistent information \- such as a name \- changes over time, but is also useful when multiple objects have the same name. The author of this chapter was once shocked to read an obituary [carrying his own name](https://obituaries.paloaltoonline.com/obituaries/memorials/dr-john-borghi?o=8288)\!

**Choosing a repository**

If data can be shared through a repository, researchers have a series of decisions to make. The first is "which?" 

Choosing the most appropriate repository is no small challenge. As described in **Table 6.7.** data repositories can be divided into several categories. 

**Table 6.7. Types of data repositories**

| Repository Type | Description |
| :---- | :---- |
| **Institutional Repository** | An archive for collecting, preserving, and sharing materials and outputs related to a given institution. An advantage of an institutional repository is that it is maintained *by the institution***,** meaning that there is local support and a degree of stability that might not be present for other options. |
| **Specialized Repository** | Archives that have been developed to collect, preserve, and make select datasets available to others. Such repositories may accept specific types of data (e.g. neuroimaging data, genetic data), specific formats or “types” of data, data pertaining to specific research topics, data arising from specific research initiatives or funders (e.g. the NIMH Data Archive), or data from specific research domains. |
| **Generalist Repository** | Archives accept data regardless of data type, format, content, or disciplinary focus. In general, generalist repositories are excellent place to deposit materials that do not fit into more specialized repositories.  |

None of these is “better” than the other and \- very often \- it makes sense for the data from a single research project to be distributed over several different repositories. But, for general guidance about where to deposit research data for the purposes of sharing, see **Figure 6.1.** 

| <img width="1600" height="1056" src="https://resize-v3.pubpub.org/eyJidWNrZXQiOiJhc3NldHMucHVicHViLm9yZyIsImtleSI6IjE2M2FscDRlLzUxNjU1MzAzOTE5MjM2LnBuZyIsImVkaXRzIjp7InJlc2l6ZSI6eyJ3aWR0aCI6MTYwMCwiZml0IjoiaW5zaWRlIiwid2l0aG91dEVubGFyZ2VtZW50Ijp0cnVlfX19" />|
| ----- |
| **Figure 6.1. Choosing a data repository** Guidance for researchers when choosing the best repository for their data. From [Borghi and Van Gulick, 2022]((https://doi.org/10.1162/99608f92.9497f68e))|

Even with the above flowchart, choosing the right repository can be a challenge. There are a an ever increasing number of specialized and institutional repositories. Certain disciplinary communities may even prefer one generalist repository over another (e.g. the Open Science Framework versus Dryad). Tools such as Registry of Research Data Repositories (Re3Data) can be helpful. But, when in doubt, look at where other members of the research community are sharing and choose the repository or repositories that work best for you and your data.

### Data Catalogs and Data Availability Statements

The data repository ecosystem is constantly growing and evolving. Data from the same project can, and often should, be deposited across multiple repositories. But for shared data to be useful, there needs to be a way to put all the pieces back together.

Over the last few years, tools like [Google Dataset Search](https://datasetsearch.research.google.com/) and the [NLM dataset catalog](https://www.datasetcatalog.nlm.nih.gov/) have emerged to help researchers find data shared by others. These tools are useful, but limited. They do not cover every repository, do not (necessarily) reveal links between datasets deposited in separate repositories, and do not (necessarily) reveal datasets with limitations or restrictions on (re)use. The other major limitation is that they do not cover data that is not shared openly - because how could they?

Like a library catalog, a **data catalog** facilitates the discovery of research data by providing a searchable and browsable collection of datasets. Many research institutions are currently in the process of developing their own data catalogs. But, at present, it is mostly up to individual researchers to keep track of and communicate where their data is shared.  This means maintaining both an internal index of where data has been saved and uploaded and also clearly communicating where data can be found through a **data availability statement** \- a short section of a research paper that outlines if, when, and how any related data can be accessed. 

> **Tool Highlight: [Data Index Checklist](https://docs.google.com/document/d/1qTkKoNBriP5bqoJWyvZl29xvjue9WJIRgCnW7ZQP3LY/edit?usp=sharing)**
>
> Useful when setting up a system for ensuring data stored internally (e.g. on lab servers) can be found, this checklist is also intended for groups who need to keep track of where they have shared data.
>
> [The checklist can be accessed here](https://docs.google.com/document/d/1qTkKoNBriP5bqoJWyvZl29xvjue9WJIRgCnW7ZQP3LY/edit?usp=sharing).

An internal data index can be relatively straightforward, consisting of several columns in a spreadsheet. This index does not have to be publicly available, but should be available to members of the research team as appropriate.

Writing a data availability statement can be challenging. Even a cursory analysis of data availability statements in the published literature will demonstrate that they are often of mixed utility[^9]. One reason for this is that these statements are often written early in the submission process, before the data is actually in a state where it is ready to be shared for the purposes of reuse. As a result, these statements may be overly vague or point readers towards repositories that do not actually include the data. 

To avoid all this, see the illustrative examples below:

**If data is shared via one or more repositories:** Provide BOTH the name of the repository and the PID where shared data can be found. For every dataset, make sure the PID actually resolves to the dataset.

*The data underlying the findings described in this paper can be accessed via the following repositories. Neuroimaging data is available on Open-Neuro (DOI: XYZ). Sequencing data is available on dbgap (Accession number: ABC). All other data is available on figshare (DOI: XYZ). The code used to clean, analyze, and visualize this data is available on Github repo, with an archived and timestamped version on Zenodo (DOI: XYZ).*
   
**If data sharing must be constrained or occur through another mechanism (e.g. via request):** Provide a description of why the data must be restricted and information about any paths for gaining access to the data, even if it is heavily restricted (e.g. data is only available to institutional affiliates, access requires signing a DUA, etc).

*Because of concerns about patient privacy, the raw data collected for this study cannot be made publicly available. This data is currently archived in secure storage. Use of this data may be granted following approval from our data access committee, any relevant institutional review boards, and other institutional offices and/or stakeholders as appropriate (e.g. Privacy Office, Information Technology, etc.) Applications, describing both how the proposed use of the data and the information security measures in place, should be submitted through our online portal (URL: XYZ). Questions about this process may be directed to the corresponding author.*

## 6.6. Giving and receiving credit

Over the last several decades, a great deal of effort has been put into elevating the status of research data as a “first class” output of the research process, one that carries similar incentives as the publication of a scholarly manuscript. After all, a well curated dataset comes after an investment of time, effort, and applied expertise and can represent a tremendous addition to the scholarly record.

The question of ownership of research data is addressed in more detail [elsewhere in this guide](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_02_defining-data#24-data-ownership), but it is worth revisiting in the context of data sharing. When depositing research data into a repository, a researcher may be confronted with a difficult question \- _what license should be applied to the data?_

In general, when sharing data in any kind of open fashion, it is best to assign as permissive a license as possible in order to facilitate the reuse of data. It may be tempting to choose a license that includes an explicit expectation that any additional use of the data will credit the initial authors (e.g. CC-BY). After all, credit in many areas of research comes through citations. But assigning restrictive licenses can limit important re(uses) of shared data.

_What happens when multiple datasets carrying this license are combined into a new dataset?_

This refers to a situation called **license stacking** (or a rights mess), in which two or more licenses have terms that cannot be legally or practically combined. For example, a CC-BY-SA grants the ability of others to use an object (such as a database) whoever they like as long as they give attribution to the authors and share any derivative works under the same license. But if that object is combined with another, that carries a CC-BY-NC license, things get messy. The latter license allows for *noncommercial* use as long as attribution is given. The restriction against commercial use is not included in the share alike license, but the derivative work must carry the same work as that original object. Oh no, brain error\!

_And what happens when copyright is ignored?_

This question may seem snarky, and admittedly it is a little bit. 

Very often it makes sense to put research data into the **public domain**, meaning that the copyright holder has relinquished any applicable copyright protections and enabled others to make use of data without restriction. Researchers should absolutely not do this if they intend use the data to support a patent or other intellectual property claim. But the processes of giving and recieving credit in most areas of science operate through other mechanisms.

In a research context, the use of a work is acknowledged through adherence to a broadly accepted norm \- Cite your sources. No scientific paper has ever been acknowledged or not aknowledged because of its license. Instead, credit is given and received through citations.

The same can be said (often) about research data.

Of course, it is always important to adhere to whatever terms and conditions may apply. But in the absence of other guidance or requirements, researchers should cite the data they use and expect that others will cite their data as well. 

## 6.7. Sharing Usable Data

Whether its shared through e-mail, a state-of-the art repository, or is available upon "reasonable request", sharing data is only worth the time and effort if data is shared in a manner that enables it to be (re)used.

The good news is that, if data is effectively managed throughout the research process, than much of the work needed to ensure that the data is usable has already been completed. The lift for sharing is thus (relatively) small.

Here, again, are the five checklist items for unsuring that shared data is usable data.

**1\. Is there a clear path for accessing the shared data?**

No matter how data is shared, it can only be used if it can be accessed. For data shared through data repositories or similar platforms, this typically involves providing a direct route to the data using a persistent identifier, accession number, or file path. For data that has to be shared in a more controlled manner, clear instructions should be provided in regards to how the data can be accessed and any terms of use. Among the many difficulties with the phrase “Data available upon reasonable request” is that it leaves a great deal of ambiguity about the mechanism through which the data is actually available and what a “reasonable” request actually entails.

**2\. Is the data shared in a form or format that would allow it to be used by others?**

As covered in the chapter on [Data Storage and Organization](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_05_saving-organizing), data should be saved in open or common file formats whenever possible. This is especially true when data is released for use by others.

**3\. Is the data sufficiently well described to allow it to be used by others?**

As covered in the chapter on [Documentation and Description](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_04_documentation) data that has not been saved alongside the documentation needed for its use has not really been saved at all. One of the great advantages of sharing data through a repository is efficiency, but if the researcher who downloads the data needs to sit with the original research team to make sense of the files, than the upload is mostly just taking up space in a server somewhere.

**4\. Are the links between the data and any related materials (or versions) defined?**

If a set of shared data is related to the conclusions described in a research paper, then a user should be able to find the dataset from the paper. The reverse is probably also true, but can be a bit trickier from a practical perspective. The locations of shared data should be properly described in data availability statements and other indices.

**5\. Is the data shared in a manner that allows credit for its use to be given and received?**

It should be! Almost every citation style has a format for crediting the use of a shared dataset and, when in doubt, a researcher can always state explicitly how they'd like their data to be cited.

## Definitions of Key Terms

**Data Availability Statement** \- A short section of a research paper that outlines if, when, and how any related data can be accessed. 

**Data Repository** is a platform that facilitates the preservation, organization, and discovery of research data. 

**Data Sharing** \- Broadly defined as making data available for use by others \- can be thought of as continuous with data management. 

* **Sharing for collaboration** \- The sharing of research data *within* the confines of a given research effort. Typically, this involves one researcher (or team) sharing data amongst themselves and with their collaborators (e.g. statisticians, other research professionals).  
* **Sharing for reuse** \- The sharing of research data *beyond* the confines of a given research effort. Most often, this refers to sharing with individuals who were not involved in the data’s acquisition, transformation, analysis, or initial publication.

**Data Use Agreement** - A contract that outlines how a specific set of data can be accessed and (re)used.

**License Stacking** - A complex situation in which the reuse of a dataset (e.g. combining one dataset with another), can lead to more and more restrictions on future use.

**Persistent Identifier** \- A digital identifier that permanently and unambiguously identifies a digital object or an individual. 

**Public Domain** - Describes circumstances when works are not protected by copyright and can be freely used, shared, or adapted by anyone.

## Further Reading

Altman, M., Borgman, C., Crosas, M., & Matone, M. (2015). An introduction to the joint principles for data citation. Bulletin of the Association for Information Science and Technology, 41(3), 43–45. https://doi.org/10.1002/bult.2015.1720410313

Ceci, S. J., & Walker, E. (1983). Private archives and public needs. American Psychologist, 38(4), 414–423. https://doi.org/10.1037/0003-066X.38.4.414

Siekevitz, P. (1957). Powerhouse of the Cell. Scientific American, 197(1), 131–144. https://doi.org/10.1038/scientificamerican0757-131

## Footnotes

[^1]:  Kingsbury, B. F. (1912). Cytoplasmic fixation. The Anatomical Record, 6(2), 39–52. https://doi.org/10.1002/ar.1090060202

[^2]:  For more on open access, see the eponymous book: Suber, P. (2012). *Open Access*. The MIT Press. [https://doi.org/10.7551/mitpress/9286.001.0001](https://doi.org/10.7551/mitpress/9286.001.0001)

[^3]:  Palade, G. E. (1953). An electron microscope study of the mitochondrial structure. *Journal of Histochemistry & Cytochemistry*, *1*(4), 188–211. [https://doi.org/10.1177/1.4.188](https://doi.org/10.1177/1.4.188)

[^4]:  Claerbout, J. F., & Karrenbach, M. (1992). Electronic documents give reproducible research a new meaning. *SEG Technical Program Expanded Abstracts 1992*, 601–604. [https://doi.org/10.1190/1.1822162](https://doi.org/10.1190/1.1822162)

[^5]:  Buckheit, J. B., & Donoho, D. L. (1995). WaveLab and Reproducible Research. In A. Antoniadis & G. Oppenheim (Eds.), *Wavelets and Statistics* (Vol. 103, pp. 55–81). Springer New York. [https://doi.org/10.1007/978-1-4612-2544-7\_5](https://doi.org/10.1007/978-1-4612-2544-7_5)

[^6]: Data sharing has been discussed in the scholarly literature for _at least_ half a century, but for an amusing take on all this that involves a proposition to trade raw data for a “a summary of employment opportunities in your area”, see Craig, J. R., & Reese, S. C. (1973). Retention of raw data: A problem revisited. *American Psychologist*, *28*(8), 723–723. [https://doi.org/10.1037/h0035667](https://doi.org/10.1037/h0035667)

[^7]:  [ICMJE Defining the Role of Authors and Contributors](https://www.icmje.org/recommendations/browse/roles-and-responsibilities/defining-the-role-of-authors-and-contributors.html)

[^8]:  This phrase is now ubiquitous in data management circles, but came to prominence in 2016 when the European Union began to include data sharing and other open science practices into scientific research initiatives (e.g. Horizon 2020, Horizon Europe).

[^9]:  For further discussion on this topic: Gabelica, M., Bojčić, R., & Puljak, L. (2022). Many researchers were not compliant with their published data sharing statement: A mixed-methods study. *Journal of Clinical Epidemiology*, *150*, 33–41. [https://doi.org/10.1016/j.jclinepi.2022.05.019](https://doi.org/10.1016/j.jclinepi.2022.05.019)
