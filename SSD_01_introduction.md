# Chapter 01: Understanding Data Management

What are we talking about when we talk about data management and data sharing? This module defines these topics in both technical and functional terms.

---

| | **Key Points for this Chapter** |
| :---- | :---- |
| 1\. | The term “data management” covers a large number of practices and strategies designed to support the usability and quality of research data over time. |
| 2\. | Everyone who works with research data is responsible for data management, though different individual researchers may have their own roles and responsibilities. |
| 3\. | Data management helps make the research process more efficient and is foundational to ensuring that the research process is ethical, reproducible, accessible, and implemented in line with applicable regulations and policies. |
| 4\. | As a practice, data management exists along a continuum. A research group may excel at one aspect of data management and need improvement on others. |

| | **Supplementary Materials for this Chapter** |
| :---- | :---- |
| [Good Data Management Principles](https://docs.google.com/document/d/1dZeyt_6qnnvjfI9PEIXbhRK1ELhfG1NS9jlAn7mFEF0/edit?usp=sharing) | This document presents each of the ten principles of Good Data Management Practice along with a brief description of each. |
| **[Good Enough Practices](https://docs.google.com/document/d/1RbdOQPJUMUKwMvxIgznEBr7_TT_MCGCCWQajCOdEJJY/edit?usp=sharing)** | Sometimes “Good enough” has to be good enough. This document provides a starting point for implementing data management practices. |

---

## 1.1. Introduction: What is research data management?

Let’s begin with with a few examples: 

A research team is exploring exciting frontiers in their field. Their methods are novel, they publish their findings in prestigious journals, and their peers hold them in high regard. Grants are funded, careers are made, and awards are won.

The team views themselves as good citizens in the sprawling, multifarious enterprise that is science. But science is done by people. People with tremendous expertise and specialized skills. People who care a lot about getting things right. Science is also a process. A process that is incremental and cumulative. But like any process undertaken by people, mistakes can happen.

In practice, these mistakes don’t always matter. Nobody might ever need that one misplaced file. That detail omitted from a description of a new method may not prevent others from using it successfully. That copy and paste error may not meaningfully affect the conclusions drawn from the analysis of a dataset. But sometimes these mistakes do matter. And when they matter, they tend to *really* matter.

*Example 1:* In the rush to meet a deadline, a team member accidentally mislabels a file. This file is then lost to the maw of the group’s digital storage system. Unfortunately, this file contains information crucial to understanding why a specific decision was made. Subsequently, the team member has to re-run their entire analytic workflow so they can give a full accounting of what they did and why. This process may take a few minutes or it may require weeks of constant effort.

*Example 2:* To meet the formatting requirements of a scholarly journal, another team member omits a small detail from the specification of a new experimental method. Because this detail is widely understood to be standard practice within the group, they believe it does not need to be made explicit. Unfortunately, when other teams try to follow the method as published, they are unable to get the expected results.

*Example 3:* After hours of wrangling a dataset organized in a spreadsheet, a third team member accidentally moves a set of values into the wrong column. This error goes unnoticed and the conclusions drawn from the ensuing analysis are published in a scientific journal. After an interested colleague asks for the data and discovers that correcting this error significantly affects the results of the analyses that support the conclusions of the paper, the work is retracted.

Everyone in the group had been following what they considered to be good scientific practice. There was no intention to delay, misguide, or deceive. But, all of a sudden, everything is in question. The progression of research projects \- and therefore publications and therefore career advancements for members of the research team \- may be substantially delayed. An individual team member \- or even the group as a whole \- may see their standing in the field greatly reduced. Results affected by errors may form the basis of new policies or recommendations. A perception that a certain area of research lacks rigor may undermine confidence in the process of science as a whole.

At the center of all this commotion is data management.

Because the term“data management” encompasses a wide variety of concerns, stakeholders, strategies, and behaviors, it can be difficult to find a common definition.

Here is how the National Institutes of Health (NIH) defines the term:

***Data management** is the process of validating, organizing, protecting, and maintaining scientific data to ensure its accessibility, reliability, and quality.*

This is, admittedly, thorough. But it is also a rather complex definition that includes a number of nuanced concepts and topics. Almost every term invoked could be the basis of its own module or guide.

So what is data management really?

Functionally, **data management** can be thought of as an umbrella, covering a large number of practices and strategies designed to support the **usability** and **quality** of research data over time. Just as research data supports research results, effective data management supports research data. Through the implementation of good data management practices and strategies, research data can be found, accessed, and used by authorized users as needed.

Data management–related practices and strategies can be thought of as being continuous with those involved in “data wrangling” and “data curation”, which similarly involve rendering sets of data into forms that ensure they can be used by researchers (and their computational tools). But data management is broader, encompassing efforts and expectations throughout the entire research process \- from the development of plans well before data is acquired through to the stewardship of data and other materials for years after the conclusion of a research effort. 

This will be emphasized in subsequent modules, but realizing the benefits of data management often requires the adoption of standards. This concept is often misunderstood, but a standard is essentially just an agreed upon way of doing something. Typically, a **data standard** includes agreed upon ways of storing, organizing, describing, and communicating about data. In some fields of science, especially those in which datasets are aggregated and reused, formal standards are quite common. In others, not so much.

Data management is not a one time activity.  Files can sometimes be backed up after the bulk of the data analysis process has been completed. Notes about what processes were implemented can be sometimes filled in after the fact. But \- to realize their fullest benefit \- data management practices and strategies need to be implemented continuously, during the day-to-day course of a research effort.

Illustrating this requires a small detour. **Table 1.01.** outlines a very general description of the research process. This is not meant to be comprehensive or descriptive of every research effort everywhere, but rather to provide a starting point for talking about data management throughout this guide.

#### Table 1.01. Phases of a research effort

| Phase | Description of Phase |
| :---- | :---- |
| **Envision and Plan** | The research team prepares to initiate a research effort. This includes gathering materials, devising strategies and systems, connecting with resources, and completing the necessary administrative steps to proceed. |
| **Generate and Acquire** | Research data is obtained by the research team. Raw data may be generated experimentally or simulated computationally. Existing datasets may also be acquired and repurposed. |
| **Process and Analyze** | Research data is acted upon so that observations and conclusions can be made. This often involves cleaning, parsing, and other forms of processing which can result in the generation of “intermediate” data files and other materials (e.g. code, documentation, etc).  |
| **Report and Share** | Observations and results are disseminated (e.g. through scholarly publications). Increasingly, this is coupled with an expectation that the underlying data will be shared concurrently (with restrictions as appropriate). |
| **Archive and Reuse** | Data is accessed, evaluated, repurposed, and expanded upon. Data may be preserved through repositories that facilitate discovery and reuse. Data is also preserved internally by the research team and/or their institution. |

Effective data management \- even in the most straightforward of projects requires action at each of these phases. Some example scenarios are given in **Table. 1.02.** 

Again, this is certainly not meant to be a comprehensive set of activities. Different teams will need to do different things. But hopefully this demonstrates how relatively simple activities \- including those related to data storage, organization, and documentation \- have to be carefully considered at every step along the way.

#### Table 1.02. Examples of data management activities 

|  | Data Storage | Data Organization | Data Documentation |
| :---- | :---- | :---- | :---- |
| **Envision and Plan** | A research team ensures that their storage systems are sufficient to retain all of the data they plan to collect. | The team establishes a standardized system for keeping track of file versions, so collaborative work can proceed smoothly.  | The team ensures every member is trained on how to follow the study protocol and maintain contemporaneous notes in sufficient detail. |
| **Generate and Acquire** | As data is acquired it is deposited into the appropriate system and backed up to prevent important information from being lost. | The team maintains a standard directory structure, so data can be located without difficulty. | The team develops a data dictionary or codebook to ensure that data files can be understood and used. |
| **Process and Analyze** | Intermediate data files and workflow materials (e.g. software, code) are properly stored and backed up. | The data is processed into a form that renders it interoperable – meaning it can be accessed and used by human researchers and computational tools | Changes made to the data as well as analyses parameters are recorded in sufficient details as to ensure data provenance.  |
| **Report and Share** | A “final” version of the data is saved, which directly underlies any results described in a published paper. | The “final” dataset is structured using an appropriate metadata schema and/or accompanied with sufficient documentation to ensure usability. | The process leading from the data to the conclusions derived from them are sufficiently described and communicated.  |
| **Archive and Reuse** | Some or all of the data is deposited into the appropriate data repository so it can be discovered and reused | The data is shared in a format that ensures others will be able to use it (e.g. common file formats). | The data is stored in a manner that ensures it is reusable over time. |

**Data Provenance**

Motivations for implementing good data management are covered in more depth in Section 1.3., but largely the answer to the question “Why do we do all of this data management stuff?” comes down to **data provenance**. If data is evidence for a scientific result, data provenance is an audit trail or chain of custody for that evidence. Data provenance describes the origin of a set of data, how it has been changed and transformed over time, where it has been, and where it is now. Breaks in this chain or trail can have consequences for a research effort that range from inconvenient but manageable to absolutely devastating for a research effort and individuals involved. 

Good data management is absolutely foundational to ensuring that data provenance is maintained. The research process can be messy. It is almost never as linear or made up in phases that are as discreet as those described in Table 1.01. Decisions made at every stage can affect not only the final research results but also what can be done at subsequent stages.  
Amid all of these paths not taken, data provenance represents how a research team ended up at their conclusions.

**Data Sharing**

Throughout these modules, data sharing is referenced as an outcome for effective data management. Topics related to data sharing will be covered in much more detail in subsequent chapters. But, defined broadly, **data sharing** is the release of data for use by others. 

Very often, this term is used as a shorthand for making data available to individuals beyond the original research team. In 2025, this can refer to making data available “openly” \- meaning without restriction as to who is able to (re)use it and for what purpose. But the term also encompasses more limited forms of sharing. Sending a dataset to a biostatistician or other close colleague is a form of data sharing. Passing data and materials to another researcher in a research group so they may continue a particular project is a form of data sharing. 

Perhaps the most common \- and most underappreciated \- form of data sharing is when a researcher shares data with *themselves*. As will become clearer in future modules, returning to a dataset after any amount of time is much more straightforward when it has been properly saved, organized, and described.

Working under the assumption that another researcher will need to find, access, and make use of a set data at some point in the future is helpful when developing and implementing data management-related practices and strategies, even if broader sharing is not possible or desired. 

## 1.2. Who is responsible for data management?

Because they do not have nearly enough work to do, the majority of research data-related regulations and policies place the ultimate responsibility for data management on a project’s primary investigator (PI). So, if you are not a PI, feel free to stop reading.

Just kidding.

Like many *many* other activities in science, data management is a collaborative effort. In practice, this means that everyone who works with a set of data is responsible \- in some way \- for ensuring that it is managed properly.

How and where to define specific roles and responsibilities related to data management and sharing throughout the research process is covered in additional detail in *other parts of this guide.* But it can be useful to make a distinction between those individuals primarily responsible for setting and monitoring data-related strategies and policies (i.e. project leadership) and those primarily responsible for implementing practices defined by others (i.e. project team members) (see **Table 1.3**). These are not wholly distinct groups of course; a primary investigator may work at the bench and analyze data, a grad student may help write new policies and procedures. These groups are also not homogenous. Different project team members may have different responsibilities and areas of focus or may even play different roles on different projects.

#### Table 1.03: Who is responsible for data management?

| Group | Select Responsibilities |
| :---- | :---- |
| Project Leadership | Setting policy Communicating practices and procedures  Monitoring and auditing Education and mentorship Responding to feedback |
| Project Team Members | Implementing practices and procedures  Providing feedback to leadership Asking questions |

In this conception, project leadership is responsible for empowering others to manage data well. It is generally not the case that data-related practices and strategies need to be developed from scratch. Many areas of research (and many groups adjacent to research) have developed standards and best practices that can be adapted and built upon. Because data management is not typically covered in formal coursework or other training, a vital role for project leaders is also mentorship \- ensuring that project team members are well versed in what they should be doing with data.

Project team members are then responsible for contributing to the broad practice of data management. This means more than simply following practices and procedures by leadership. Because they are actively involved in the day-to-day practice of storing, organizing, and describing data, team members should proactive communicate with leadership about challenges and opportunities. They know what is working and what is not working.

In scientific research, there are a number of stakeholders beyond the research team who are responsible for some aspect of data management. A given research area may also have its own norms, expectations, and standards related to data management and sharing. Research Institutions also have their own responsibilities related to research data, including those that arise from research ethics, laws and regulations, and contractual obligations (i.e. those made with research funders). 

As a result, data management is also an administrative process \- often one that involves institutional offices and groups involved in research compliance, protection of research participants, privacy, information technology, and many others. Navigating this landscape can be challenging, hence the how-to guides, and workflows developed as part of the following modules.  
                                                                                                                   

## 1.3. Why do all this? \- Motivations for data management

As will quickly become evident moving forward, properly managing scientific data takes time and effort. There’s a learning curve and, often, there is a financial cost. So why bother? 

It is not a (totally) unfair question. Scientific research, especially academic scientific research, often progresses through the publication of scientific papers. The published record of science (generally) persists as time passes, technology evolves, and labs turn over. But individual datasets or the documentation describing their provenance may not. Given limited time and resources, it is not (totally) surprising that data management is sometimes regarded as a secondary concern. 

But it should not be.

*Trustworthiness* in science is a constantly moving target. A few years ago, reverse engineering a fraudulent dataset to support a claim would have required considerable expertise and a substantial amount of time and effort. Now it can be done in less than a minute by prompting a large language model. Amid a changing global and political climate, practices and strategies once thought to be standard are now seized upon to justify funding cuts and the denial of vital scientific evidence.

The point is not that every scientist needs to feel more anxiety about making small mistakes or that any single researcher needs to become an expert in every aspect of data management. Small mistakes are inevitable. But rather, every researcher needs to pay attention to how they are supporting their data. 

Collecting and analyzing data is not *a part* of the process of science. These activities are not simply precursors to publishing a journal article. Collecting and analyzing data *are* the process. Even the most sophisticated techniques and methods don’t amount to much if the records of what was done and what happened are not properly maintained. 

Science is built on data. This data comes in all sorts of shapes, sizes, and formats. Data is what supports scientific hypotheses and results. Supporting science means supporting data. With this in mind, data management can be thought of as being important at two levels:

1. For individuals and teams who need to keep track of data, materials, processes, and procedures over the course of a given research effort.  
2. For the broader research enterprise that is invested in establishing the integrity of the research process and the reusability of data sets and other products of the research process.

Beyond these, research data management lies at the intersection of a number of issues. These include, but are not necessarily limited to the following:

**Research Ethics**

Sensitive data will be discussed in much more detail elsewhere in this guide, but certain data must be protected against unauthorized access and use. The reasons for this range from protecting endangered species to protecting national security, but the relationship between data management and research ethics is perhaps most easily illustrated with the case of data derived from human research participants.

Upholding the rights of human research participants must be centered in all research activities. That is not (just) a matter of regulation and expectation, but a matter of ethical responsibility for all researchers. Not only should protecting privacy and other rights for human participants be  centered in the implementation of data management-related activities, but proper data management is also vital to conducting ethical research.

Effective data management minimizes the risk posed to participants through the proper storage and treatment of sensitive information. Research participants contribute their time and, in many cases, much more to a given research effort. Proper data management helps to maximize the value of these contributions by enabling data to be used and reused. 

Of course, facilitating the usability (or reusability) of data from human participants merits careful ethical consideration. Research data is a resource and, with any resource, there is potential for iniquity and exploitation. 

**Efficiency and Team Science**

Preventing the loss of data is probably the most immediate benefit of implementing a data management strategy. All storage media have a rate of failure (more on backup procedures in a future chapter), but there are many ways to lose data; files can be misplaced, versions can be confused. details can be forgotten. Such a loss often means that an individual researcher or research team may need to spend time and other resources redoing or reconstructing their work. Depending on the circumstance, this might be a substantial or even impossible endeavor.

Data management also helps the collaborative aspect of scientific research proceed efficiently. Scientific research is a process and that process proceeds much more efficiently when everyone involved can find and use the data they need. The most common collaboration in a given research effort is an individual researcher with their future self \- the version of themselves that has not opened a particular file in a couple of days (or months or years). But the same strategies and practices that will help that individual researcher find and use the data they need also do the same for other members of their research team (labmates, biostatisticians, etc), and the research community more broadly.

**Research Quality**

Over the last several decades, much has been written about the reproducibility of scientific findings. The term has proven somewhat difficult to define, but efforts to address **reproducibility** are generally concerned with establishing the credibility, reliability, and validity of scientific research. Addressing the conduct of “good science” is well beyond the scope of this guide and a subject heavily intertwined with politics, ethics, philosophy, and other areas. But assessing the “quality” of research \- however that may be defined \- is quite difficult when the data and materials that support a result have not been properly managed.

This is not to raise the specter of fraud and scientific misconduct. Intentional breaches of trust do happen, of course. But they are exceedingly rare. But, it would be a disservice to narrow the utility of data management to just safeguarding against accusations of research impropriety. Scientific findings are supported by data. So any discussion of “quality” in the context of scientific research must also account for how well that data is supported.

**Accessibility**

These days, it is not common to consider the publication of scientific journals as a step forward for the accessibility of science. But, starting in the 1600s and beginning in earnest in the 1800s, this development in scholarly publishing meant that discussion of scientific results was no longer confined to the correspondence between individual scientists. 

There are a variety of processes for making datasets and other materials accessible to others. These processes, like the sharing of journal articles, is enabled by the development of tools and technologies that have greatly changed how science is communicated and who can participate in the research process.

The term **open science** covers a variety of efforts focused on making scientific research more transparent and accessible. Though it is frequently used to refer to efforts aimed at ensuring access to tools and research products (e.g. open access for journal articles), open science also encompasses efforts to ensure that the scientific enterprise is inclusive and equitable. 

There is an increasing recognition that data should be a “first class” research output in and of itself \- evaluated, disseminated, cited, and valued in a similar standing as publications. But, beyond just the incentive system of academic science, making data available (and accessible) has a number of benefits. For the individual researcher, sharing data and other materials can lend additional support to research results, as they can be verified and even expanded upon by others. Data sharing also enables data reuse, which greatly benefits the research enterprise as a whole, as datasets can be examined, combined, and used for the development of new tools, methods, and research and educational efforts.

**Regulations and Requirements**

Probably the most immediate motivation for data management is that it is required by the entities that support the scientific research enterprise. For example, at Stanford University, data management is written into the institution’s data retention policy and Research Policy Handbook.

 >> *“The PI is responsible for the collection, management and retention of research data. PIs should adopt an orderly system of data organization and should communicate the chosen system to all members of a research group and to the appropriate administrative personnel, where applicable.”*  [Stanford Research Policy Handbook (RPH 1.9)](https://doresearch.stanford.edu/policies/research-policy-handbook/conduct-research/retention-and-access-research-data)

In the United States, federal agencies that fund research \- such as the National Institutes of Health (NIH) \- have begun to require that researchers detail how they plan to manage and share data as part of grant proposals. These requirements will be covered in detail in a future module, but it is worth noting here that the contents of these plans become terms and conditions of any subsequent award and that there is an explicit expectation that researchers will “maximize appropriate data sharing” when developing their plans.

## 1.4. Good Data Management Practice

One last point is important to emphasize: Data management is not an all or nothing endeavor.

Data management is a continuous and multifarious process, involving many decisions and actions over the short, medium, and long term. It can be overwhelming. But the goal of this guide is not to assert that every researcher needs to become an expert in every single data-related practice and strategy. Given how rapidly these areas are evolving, this is likely not even possible.

But it is also very likely that any researcher reading this guide has or will have an experience where they find themselves in a setting where practices and strategies related to data management are still being developed.

There are many research groups who have thought carefully about how data is managed and have adopted an excellent set of systems and checks to match. There are also groups who may have a “way of doing things” that is neither well documented nor particularly standardized between (or even within) different projects. 

It is also not that a research group has either “good” or “bad” data management overall. A group may be very sophisticated in their practices related to one aspect of data management \- such as storing and backing up data \- but have much less defined practices for others.  
So what can be done?

Well, there are a few approaches that an individual or research team can take to support their data through data management.

**Manage what can be managed**

The first approach, to manage what can be managed, is outlined in **Table 1.04.** So far data management has been discussed as a collaborative activity, one that involves multiple members of a given research team. This is ideal and good data management and team science are mutually beneficial. But an individual researcher may or may not be empowered to prescribe data management activities for the broader team of which they are a part. In such a case, that individual researcher can only ensure that they themselves are implementing good data management.

#### Table 1.04: Levels of Data Management

| Level | Best Case Scenario |
| :---- | :---- |
| **The individual researcher**  | Data management is a continuous process. Standardized practices should be implemented throughout the day-to-day work of a research project.  |
| **The research team** | Data management is a team effort. The maintenance of specific, informative, and up-to-date documentation about how data should be managed and shared will help work to proceed efficiently. |
| **The research discipline** | Data management facilitates data reuse across the field. In many research disciplines, specific data management-related standards have been adopted in order to foster downstream reuse of shared data. |

Though standards for certain types of data and research areas have been developed and implemented to great success, this is certainly not a universal phenomenon. If a more formal data standard has not been developed or widely adopted, a research team may need to develop their own *standardized practices* \- agreed upon strategies related to storing, organizing, and describing data.

**Make incremental improvements**

One of the reasons this guide is so long is because data management encompasses a wide range of activities, each with their own considerations and vocabulary. So much so that sometimes the same word can mean slightly different things \- a *repo* in the context of a tool like Git is not exactly analogous to a *data repository* as described by individuals working in the broader context of data sharing, for example.

It is unlikely that a single researcher can necessarily be an expert in all of these activities and sometimes some activities might need to take precedence over others. **Table 1.05** is a rubric of sorts that illustrates this in detail.

#### Table 1.05: Assessing data management activities

|  | Ad hoc | One Time | Continued | Optimized |
| :---- | :---- | :---- | :---- | :---- |
| Planning | When it comes to data, the team has “a way of doing things” that is not documented in detail. | There are plans for some data management activities, but they may not be followed by everyone. | Data management is included in standard operating procedures (SOPs) followed by the team. | Plans and SOPs are in line with or improve upon community standards. Plans are revisited regularly. |
| Saving and backing up | Data is not saved consistently. Important information may be lost. | Important data is saved, but is backed up inconsistently or at the end of a project. | Data is saved and backed up regularly and as a matter of course in line with SOPs. | Data is stored in line with community standards and with future (re)use in mind. |
| Organizing | Data is not organized consistently. Important information may be hard to find. | Data is typically organized after the fact so it can be found and used in the future. | Data is kept organized throughout the project in line with SOPs. | Data is organized in line with community standards and with future (re)use in mind. |
| Processing and Analyzing | Because documentation is not maintained consistently, steps often need to be repeated. | Documentation of the contents of data files and data-related processes is created retrospectively. | Documentation is maintained for data related files and processes throughout the project and in line with SOPs. | Documentation is maintained in line with community standards and with future (re)use in mind. |
| Archiving and sharing | Data from past projects is not saved consistently, making sharing difficult. | Related procedures are decided and implemented on a case by case basis. | Data is archived and shared in line with SOPs. | Data is preserved and shared in line with community standards and with future (re)use in mind. |

Sometimes it might only be possible to improve data management by a small amount, but even something as seemingly minor as finding a way to continuously and automatically back up data represents a step in the right direction.

**“Good enough” sometimes has to be good enough**

Ok, but where to start?

When developing data management practices and strategies, even something as simple as considering options for storing a dataset can lead down a very deep rabbit hole.There’s file formats to consider, and storage media, and regulations, and policies, and budgets…

There are quite a few documents available that cover “best practices”. Many of them are listed in the *Further Reading* section of this and other modules. But, while the majority of them give excellent advice, the reality on the ground is often a lot messier than is portrayed in these practice guidelines and recommendations.  “Best practices” in research data management is also a constantly moving target.  The ecosystem of tools, resources, and repositories is constantly and rapidly evolving. Different research communities have different priorities and expectations. 

So let’s get back to basics.

Throughout these modules, such ten basic principles of data management will be discussed and expanded upon. Organized under the umbrella of **Good Data Management Practices,** these principles are not a set of regulations. They are not even really a set of expectations. Instead, they are a way of thinking about how to support research data in the context of twenty-first century science.

These principles are:

1. High quality data and high quality science require effective data management.  
2. Effective data management requires research data to be defined thoroughly and broadly.  
3. Managing data requires understanding and addressing issues related to risk.  
4. Data management is a set of practices and strategies, not (just) a set of tools.  
5. Data management practices and strategies should be standardized and routine.  
6. It takes planning and communication to manage data well.  
7. Managing data requires managing documentation and metadata.  
8. All data must be managed, but not all data necessarily needs to be shared (openly).  
9. Effective data management requires both commitment and a range of skills.  
10. Sometimes “good enough” has to be good enough.

These principles form the basis of much of the content of this guide. In fact, every module of this guide expands upon at least one. 

For more on this framework, see the following two primers:

---

**PRIMER:** [Good Data Management Principles](https://docs.google.com/document/d/1dZeyt_6qnnvjfI9PEIXbhRK1ELhfG1NS9jlAn7mFEF0/edit?usp=sharing)

This document presents each of the ten principles of Good Data Management Practice along with a brief description of each.

**PRIMER:** [Good Enough Practices](https://docs.google.com/document/d/1RbdOQPJUMUKwMvxIgznEBr7_TT_MCGCCWQajCOdEJJY/edit?usp=sharing)

Sometimes “Good enough” has to be good enough. This document provides a starting point for implementing data management practices.  

---

While perusing the remainder of this guide, remember:

No matter how revolutionary your hypotheses... 

No matter how robust your designs...

No matter how innovative and complex your analytical pipeline...

...You still need to be able to find and make use of your data.

**Good data management is an essential part of good research practice.** 

**Good Luck\!**

## Definitions of Key Terms

**Good Data Management Practice \-** A way of thinking about the support of research data in the context of twenty-first century science. Includes ten principles related to how data should be defined and how data management should be incorporated into research processes and workflows.

**Data Management** \- Strategies and practices related to the storage, organization, and description of research data. The focus of data research data management is ensuring accessibility, reliability, and quality. As a shorthand, it can be useful to think about data management as processes related to ensuring that data is usable.

**Data Provenance** (also sometimes referred to as “data lineage”), \- The documented trail that describes the origin of a piece of data, how it has been changed or transformed, where it has been moved to, and where it is presently. 

**Data Quality** \- A broad concept that refers to the degree to which a set of data is fit for its intended purpose. Highly related to data management, but also includes issues more related to methodological rigor.

**Data Sharing** \- The release of data for use by others. This includes forms of sharing that are relatively restricted (who data is shared with, what they users are able to do with shared data, etc) and more open forms of sharing (e.g. sharing of data through a publicly accessible repository. 

**Data Standards** \- Agreed upon ways of organizing, structuring, and/or describing a particular form of research data.

**Open Science** \- An umbrella term for a variety of efforts aimed at making scientific research more transparent and accessible. In this guide, we are mostly focused on activities related to the outputs of the research process (datasets, code, etc), but the term also encompasses efforts to ensure that the scientific enterprise is inclusive and equitable.

**Reproducibility** \- Broadly refers to efforts related to ensuring reliability, validity, and credibility of scientific research. Somewhat ironically, the meaning of key terms and definitions related to “research reproducibility” are not standardized across the scientific research enterprise. Throughout this guide, we generally use the term to refer to **methods reproducibility** (the provision of sufficient detail about study procedures so that they can be \- theoretically or actually \- exactly repeated).

**Usability** \- In the context of data management and sharing, this refers to an ability to open, understand, make use of, and build upon a set of data. In the context of biomedical science, “re-use” encompasses a large number of potential activities, including using a dataset for education and training (of both human researchers and algorithms), testing new hypotheses (which can involve combining multiple extant datasets), and more.

## Further Reading

Briney, K., Coates, H., & Goben, A. (2020). Foundational Practices of Research Data Management. Research Ideas and Outcomes, 6, e56508. [https://doi.org/10.3897/rio.6.e56508](https://doi.org/10.3897/rio.6.e56508)

Ellis, S. E., & Leek, J. T. (2018). How to share data for collaboration. The American Statistician, 72(1), 53–57. [https://doi.org/10.1080/00031305.2017.1375987](https://doi.org/10.1080/00031305.2017.1375987)

Goodman, S. N., Fanelli, D., & Ioannidis, J. P. A. (2016). What does research reproducibility mean? Science Translational Medicine, 8(341), 341ps12. [https://doi.org/10.1126/scitranslmed.aaf5027](https://doi.org/10.1126/scitranslmed.aaf5027)

Wilson, G., Bryan, J., Cranston, K., Kitzes, J., Nederbragt, L., & Teal, T. K. (2017). Good enough practices in scientific computing. PLoS Computational Biology, 13(6), e1005510. [https://doi.org/10.1371/journal.pcbi.1005510](https://doi.org/10.1371/journal.pcbi.1005510)
