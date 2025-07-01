# Documentation and Description 
| [Last Chapter - Planning for Data Management](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_03_Planning) | [Back to the Table of Contents](https://johnborghi.github.io/Supporting_Scientific_Data/) | [Next Chapter - Data storage and organization](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_05_saving-organizing) |

## Chapter Summary

If it is not documented, it did not happen. This chapter covers strategies and processes related to developing protocols, recording research workflow, and documenting the contents of specific data files.

This chapter is built on the principle that managing data requires managing metadata.

| [Principles of Good Data Management Practice](https://johnborghi.github.io/Supporting_Scientific_Data/supplements/SSD_good-dm-practice) | ["Good Enough" Practices in Data Management](https://johnborghi.github.io/Supporting_Scientific_Data/supplements/SSD_good-enough) |

|  | Key points for this chapter |
| :---- | :---- |
| 1\. | There are three major types of documentation that need to be carefully created and maintained during a research project: Documentation of process (e.g. protocols and pipelines), contemporaneous notes (e.g. lab notebooks), and documentation of structure and content (e.g. data dictionaries). |
| 2\. | Document more than you think is necessary, in greater detail than you think might be necessary. |
| 3\. | Documenting what should happen, through an SOP or protocol, provides a research team with a guide that can make the research process more efficient. |
|4\. | Documenting what actually happened, through a document like a lab notebook, is essential for establishing data provenance.|
|5\. | Data that is saved without the documentation necessary for its use has not been effectively saved. 
| 6\. | Documentation is a type of metadata. As such, it should be organized, stored, and archived alongside any relevant datasets and other materials.  |

|  | Supplementary materials for this chapter |
| :---- | :---- |
| [Chocolate chip cookie recipe](https://docs.google.com/document/d/1aGvheTT4Di5d5pjcceO_ukUOWWrn4kpbkpeDLJp7I7U/edit?usp=sharing) | By far the most tangential supplementary material in this whole guide, this is literally just the author’s recipe for chocolate chip cookies. |
| [SOP Template](https://docs.google.com/document/d/1ATWE-zzJoMjR9dumo_e3fOROabIrvRct/edit) | A template for writing a Standard Operating Procedure. The example given is a very important activity in the scientific research enterprise, making a decent cup of coffee. |
| [ReadMe Template](https://docs.google.com/document/d/15lOyAQZIkex0aySqZ4giNlXJ-lcN00-NMWGd1wjX5IE/edit?usp=sharing) | A template for writing a readme file that describes the contents of a dataset. |

## 4.1. A Meta Conversation about Metadata

The esteemed communicator of science Carl Sagan once quipped, “If you wish to make an apple pie from scratch, you must first invent the universe[^1].” 

In its original context, this was meant to reflect the relationship between chemical elements and the life and death of stars. With apologies to Carl Sagan, this same sentiment also describes what it is like to look up recipes online. 

Looking up a simple recipe for chocolate chip cookies often involves scrolling past paragraphs and paragraphs of preamble. This is largely due to search engine optimization rather than the physical properties of the universe. But this phenomenon is particularly grating when, after scrolling for so long, the actual recipe is missing important details. It may be interesting to learn about the life and times of Ruth Graves Wakefield, who invented chocolate chip cookies very much not by mistake in the late 1930s. But that’s not very useful if the recipe does not specify a baking time or temperature.

This is not a guide to making apple pie or chocolate chip cookies. But a good recipe and a study protocol *are* roughly analogous. Ideally both should be legible, complete, and easily accessible. Just don’t run your cookie dough through gel electrophoresis.

### Types of Documentation

To ease the transition from chocolate chip cookies to documentation and metadata, please see the most tangential supplement in this whole guide \- the author’s recipe for [chocolate chip cookies.](https://docs.google.com/document/u/0/d/1aGvheTT4Di5d5pjcceO_ukUOWWrn4kpbkpeDLJp7I7U/edit)

Anyway, onto the ontologies…

The methods section of a research paper provides a thorough description of how an experiment was done and a clear rationale for why specific experimental procedures and parameters were chosen and implemented. The outcome of all these activities and decisions are then described in the next section, the results section.

The structure of a research paper may seem too rudimentary for a guide on data management and sharing, but methods and results sections (and scholarly publications more broadly) are a form of **documentation.** Documentation refers to recorded information that is used to describe or explain something. Ideally, a reader of an article’s methods and results sections should be able to evaluate and follow the complete workflow that led up to the paper’s conclusions. 

In practice, things are not always quite this straightforward. Because of space limitations and other considerations, important details can occasionally be left out of a published paper. A particular parameter or decision may be left out because it is assumed to be too elementary or common knowledge. Such exclusion may or may not affect other researchers as they attempt to follow or build upon the described workflow. If such an exclusion is present in internal instructions maintained by the lab, it may or may not lead to frustration and delays as researchers attempt to follow a procedure without all of the necessary information.

All of which is to say, an absolutely vital part of good data management is maintaining good documentation. Documentation comes in a variety of shapes and sizes, so much so that this chapter is divided into three parts.

1. Documentation of process  
2. Contemporaneous documentation  
3. Data-level documentation

This typology is not necessarily complete and the differences between each type can be fuzzy and context dependent. Different areas within biomedical science may also have different standards and expectations for different forms of documentation. But two statements hold true for all three.

` Document more than you think is necessary, in greater detail than you think is necessary. `

` If it is not documented, it did not happen. `

### Metadata Schemas and Ontologies

Before getting into the details of how to develop and maintain each “type” of documentation, it is worth delving into the broader category of metadata.

The term **metadata** generally refers to information *about* data. Metadata may describe, explain, or facilitate the use of an element of data (e.g. a specific file or even specific data) or the dataset as a whole. Maintaining good documentation is often the best way for a research team to establish good metadata for their work. 

Like “documentation”, there are different types of metadata and individuals with different roles within the scientific research enterprise may use the term differently. Some may use the term, very technically, in the context of formalized standards and schemas for describing a set of data. This form of metadata is very important when data needs to be easily discoverable and interoperable.

The remainder of this chapter takes a slightly different angle on documentation and description and the importance of metadata is discussed further in the chapter on data sharing. But, before jumping into protocols and data dictionaries, it is worth a slight detour into the more formal side of things.

Here is an example: 

Any research team working with medical images has likely encountered images in DICOM format. A DICOM image consists of two parts, the medical image itself (i.e. pixel intensity data for the image in question) and a “header” which contains the image’s metadata (i.e. information about how the image was acquired). 

| <img width="400" alt="Image" src="https://github.com/user-attachments/assets/8a00254c-645b-4d2c-9344-5fb996c9dfff" /> | 
| ----- |
| **Figure 4.1.** An image of a structural MRI of a human brain.  With the conversion of this image from DICOM to JPEG, the metadata stored in the header has been lost. It is an image of the author’s brain amidst a previous career as a cognitive neuroscientist, but the exact parameters used in its acquisition have been lost to time. It’s a nice picture for presentations, but no longer valuable as a piece of research data.  |

As shown in **Figure 4.1.**, both parts are needed to use the image as part of a research workflow.

The metadata stored in the headers of DICOM images are organized in a standardized way into groups of data elements. For example, group “0010” contains information about the patient, with tag “0010-0030” containing the patient’s date of birth. Group “0018” contains information about how the image was acquired, with “0018-9005” providing the name of the pulse sequence used. 

This type of formal organization of metadata is called a **metadata schema.**

Here’s another example: If you have ever scrolled through a research article and found a list of keywords, these are also metadata and are largely meant to help readers find articles of interest. 

The problem with article keywords is that they tend to be free text. With apologies to all the linguists out there, language is complicated. Authors may use different words to describe the same thing. Amyotrophic lateral sclerosis (ALS), “Lou Gehrig's disease”, “motor neurone disease (MDS)”, and “Charcot’s disease” have all been used in different places or at different times to name the same condition. 

The same term may also describe very different things. A “tear” could refer to a damage done to a muscle or to the liquid secreted by lacrimal glands. Synonyms, homonyms, and lack of standardization in language can make things difficult in contexts where precision is needed.

What is needed is an agreed upon set of terms with precise meaningings that relate to each other in precise and agreed upon ways.

All the way at the bottom of a standard PubMed entry is  a list of MeSH terms. MeSH (Medical Subject Headings)[^2] is a controlled vocabulary produced by the National Library of Medicine. MeSH is used for indexing, cataloging, and searching of biomedical and health-related information. The MeSH term for ALS is “Amyotrophic lateral sclerosis” and, in the MeSH hierarchy, this term falls under broader terms including “Spinal Cord Diseases”, “Motor Neuron Disease”, and “TDP-43 Proteinopathies”. MeSH is very helpful when doing literature searches because each term has a specific meaning and the relationships between terms are well defined. 

This type of organization, shown in **Figure 4.2.**, is called an **ontology**.

| <img width="510" alt="Image" src="https://github.com/user-attachments/assets/c4c8881f-c699-4006-9d55-aa6884dc6a0d" /> | 
| ----- |
| **Table 7.2.** A segment of the MeSH hierarchy containing the term “[Amyotrophic Lateral Sclerosis](https://www.ncbi.nlm.nih.gov/mesh/68000690)”. Note that it is nested under the category “Motor Neuron Disease” which is itself under “Neuromuscular Diseases”.  | 

When it comes to metadata, one size does not fit all. The metadata that is important for a dataset that includes medical imaging is not going to be the same as the metadata that is important for an unpublished manuscript describing Cuban flora (more on this latter example at the end of this chapter). 

But in all areas of scientific research, data provenance is an absolutely vital and foundational piece of metadata: Where did this data come from and how has it changed over time?

## 4.2. Documentation of Process \- What should happen?

Good Data Management Practice includes a broad, workflow-based, definition of scientific data. Under this conception, research data encompasses not just the materials that are used and produced as data is collected, transformed, and analyzed but also information about *how* those activities were undertaken.

Documentation of research-related processes is vital for several reasons:

1. It ensures that a research team is applying the same processes when appropriate.  
2. It ensures that other researchers will be able to replicate the same processes.  
3. It helps account for analytic flexibility and other research-related decisions.  
4. It helps account for any irregularities in the data.

The chapter covering [Planning for Data](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_03_Planning) covers the development of **Standard Operating Procedures (SOPs)**. But, if you haven’t made it over there yet or need a refresher, an SOP is simply a document that describes the precise steps for doing a task. 

> **Tool Highlight: [Protocols.io](http://Protocols.io)**
> 
> Even the most detailed SOPs are only useful if they have been effectively shared. Developing and sharing SOPs do not require any complex tools, a simple document template and agreed upon strategy for storage and training may suffice.
> 
> For a more novel solution, [Protocols.io](http://Protocols.io) is a specialized platform for documenting, adapting, and sharing methods, protocols, and SOPs.
> 
> Using this tool, documents can be shared privately with collaborators and team members or publicly with a persistent identifier (a digital object identifier or DOI) to enable straightforward citation and reuse.
> 
> To see an example of a citable protocol: Borghi, J.A, (2021). *Coffee Protocol*. [https://.doi.org/10.17504/protocols.io.bw7yphpw](https://.doi.org/10.17504/protocols.io.bw7yphpw)

The utility of SOPs goes beyond data management, of course. A research team may have SOPs for data collection procedures, SOPs for cleaning data, SOPs for all sorts of things. Really, SOPs can be created for any activity that needs to be performed in the same way over and over. 

The image presented in Figure 4.1. was originally acquired as part of a research study involving functional magnetic resonance imaging, a technique with a very high degree of analytic flexibility[^3]. Under those conditions, specificity about what procedures and what parameters need to be used as a research group is acquiring, processing, and analyzing data is absolutely vital. 

> **Tool Highlight: [SOP Template](https://docs.google.com/document/d/1ATWE-zzJoMjR9dumo_e3fOROabIrvRct/edit?usp=sharing&ouid=118445803869398413021&rtpof=true&sd=true)**
> 
> In settings where there are less formal requirements related to documenting research processes, the best format for documenting and communicating standard operating procedures is the one that works for the research team. 
> 
> The best way for teams or individuals to use this template is use it as a starting point for systematizing their routine practices. The goal is not to be evaluative. The template uses the brewing of coffee as an illustrative example and there are many, many ways to brew a worthwhile cup of coffee. This is just a format for getting started.
> 
> But even in circumstances where there is slightly less space for flexibility, prospectively developing documentation about the steps to be taken helps to increase efficiency, allows for procedures to be reviewed, and \- most importantly \- stands as a guide to ensure that members of the research team are on the same page.

### Protocols

Standard operating procedures related to data acquisition, processing, and analysis are often referred to by another name \- **experimental protocols.** Protocols are the precise steps that need to be followed for a particular procedure or for a particular study. In a social science experiment, there may be a protocol that dictates exactly what a researcher should say to a participant. For techniques used by groups across a field of research \- such a western blotting[^4] \- there may be published protocols that are commonly used and adapted as needed.

An experimental protocol can be distinguished from a **study protocol**, which is a thorough description of a research project that includes information about its objectives, design, methodology, and organization. A study protocol can be thought of as a blueprint or workplan for a research study, including information about the implementation of specific activities (i.e. experimental protocols) as well as details about how reliability, validity, and regulatory compliance will be maintained.

As shown in **Table 4.1.**, these documents can often be quite comprehensive. This is because such a protocol is reviewed and evaluated, depending on the work to be done, by an institutional review board, an animal care committee, the research team, or potentially by other experts (e.g. biostatisticians, regulatory experts, bioethics experts, etc) before the study is allowed to begin. Only after it is approved, does it subsequently act as a guide for the research team as they proceed.

#### Table 4.1: Elements of a Study Protocol

| Element | Description |
| :---- | :---- |
| Background and Rationale | The reason for conducting the research study, including references to previous research on the topic. |
| Research Objectives | Succinctly, these are the aims of the study.  |
| Participant Selection and Recruitment (For human subjects research) | The population that will be studied, including inclusion and exclusion criteria as well as how they will be recruited for the study. |
| Research Design and Procedures | The specifics of the research design, tools and study measures that will be used (e.g. surveys, devices, etc), and any measures taken to reduce bias. |
| Statistical Analysis | The methods by which the data will be scrutinized in order to address the research objectives. This includes sample size justifications, methods for managing missing data, and the planned statistical procedures. |
| Data Management | How data will be handled, including how it will be saved, protected, organized and deaccessioned as needed. |
| Data and Safety Monitoring | How incoming will be monitored to ensure its quality and, when applicable, the safety of the participants. |

Outside of a few notable examples, (e.g. clinical trials) such meticulously thorough protocols \- encompassing every aspect of a research project \- are rare. A strong statement about the value of pre-registration or exploratory research or any other approaches is beyond the scope of a guide on data management. But, when it comes to ensuring all team members are on the same page about how to accomplish a specific task, it is difficult to overstate the utility of good documentation.

Extremely detailed instructions for developing good study protocols for clinical research studies can be found within Good Clinical Practice Guidelines[^5] and templates are available from a variety of sources, including the NIH[^6].

In writing protocols: Document more than you thin is necessary, in greater detail than you think might be necessary.


## 4.3. Contemporaneous Notes \- What Happened?

A detailed protocol for making chocolate chip cookies is a great start to a nice evening. But if the cookies come out burnt and full of peanut butter, questions may be asked about what transpired as the protocol was put into practice. 

Alternatively, lets say a researcher has come to a really amazing result. Amid mentally composing their Nobel speech while still sitting in the lab, the first question they will be asked is "How did this happen?"

Most often, the best tool for answering such questions is a record that was maintained contemporaneously. Contemporaneous documentation complements documentation of process. The former addressing “What actually happened?” to the latter’s “What was supposed to happen.”

In scientific research, such documentation often take the form of **lab notebooks**. Different communities within science have different norms but, in general, a lab notebook can be thought of as a record of the research activities. In fields where the notebook is the _primary_ record of the research process, such as pharmaceutical research, there is truism, "If it is not documented, it did not happen." This chapter is aimed primarily at the notebook as a part of Good Data Management Practice, but notebooks can also be important when trying to establish intellectual property.

As shown in **Table 4.2.**, there are many different “types” of lab notebook. Each has their own strengths and weaknesses. The “best” notebook is whatever works best for a particular research group.

### Table 4.2. Types of Lab Notebooks/Contemporaneous Documentation

| Type of Lab Notebook | Description |
| :---- | :---- |
| Paper Notebooks | Physical documents \- often bound, with numbered pages, and featuring notes and observations written in per \- that researchers use to describe research-related activities in sufficient detail as to allow others to replicate their steps. In some settings, the physical notebook is the original record of data. This is the lowest tech option, but it is difficult to argue with how enduring pen and paper are as a storage medium. |
| Electronic Lab Notebooks (ELNs) | Software tools that replicate and expand upon the functions of a paper notebook. In general, an ELN will be easier to search, back up, and complete collaboratively than a paper notebook. Some options even have features that facilitate lab management (e.g. keeping track of supplies). ELN’s do come with a learning curve and are subject to the same problems as any other piece of software (e.g. obsolescence, interoperability, etc). |
| Computational Notebooks | If a paper notebook is used to record what happened as an experiment was conducted at a lab bench, a computational notebook can act as a record of how data was processed and analyzed. At their core, computational notebooks are interfaces that capture the whole of a computational process- from the code, to the documentation, to the results. |
| Notes on Scraps of Paper | Better than nothing, but subject to all sorts of problems. Not every researcher in every setting needs to use the same style of laboratory notebook, but it is always worth having a conversation about what is necessary and sufficient. |

A data scientist writing code to process and handle a massive dataset will likely have different preferences and needs related to their contemporaneous documentation than a chemist doing work at a lab bench. While individual notes on scraps of paper are (maybe) better than nothing, it is always worth discussing how this documentation should be maintained. 

In general, this type of documentation should be developed at a level of specificity that would enable a person with similar expertise to follow and potentially follow what happened over the course of a research process. 

**Table 4.3.** included additional information about the qualities of good contemporaneous documentation. These are adapted from **Good Documentation Practice**, a term used by the pharmaceutical and manufacturing industries to describe the creation and maintenance of documentation.

#### Table 4.3. The Qualities of Good Documentation

| Quality of Good Documentation | Description |
| :---- | :---- |
| Attributable | The activities described in contemporaneous documentation should be traceable to a specific person, data, and (as applicable) place. |
| Legible | Contemporaneous documentation should be easy to follow,, by both current and future readers. |
| Contemporary | Information and observations should be documented as soon as possible (i.e. as events or happening or as soon as possible afterwards). |
| Original | As with data, the provenance of notebooks and other forms of documentation should be maintained. |
| Complete and Accurate | The information recorded should represent what really occurred. Information should not be deleted or changed without some sort of record. |
| Organized | Information should be included in the expected sequence and/or format.  |
| Enduring and Available | Documentation and data should be accessible and usable as needed, both immediately and in the future. |

## 4.4. Documentation of content 

Take a look at the dataset below (**Table 4.4**. Without additional information, it is nearly impossible to understand the meaning behind these numbers. 

Adding additional information, such as column headers, could enable subject matter experts to make some educated guesses about the contents of each cell. However, additional information would still be needed to ensure that these assumptions are correct.

**Table 4.4. A Poorly Managed Dataset**

| variable001 | variable 002 | variable003 | variable004 | variable005 | variable006 |
| ----: | ----: | ----: | ----: | ----: | ----: |
| 001 | Group 1 | 2024-03-15 | 1023.78 | 1891.42 | 867.64 |
| 002 | Group 2 | 2024-03-19 | 1147.21 | 1578.9 | 431.69 |
| 003 | Group 1 | 2024-03-21 | 1309.87 | 1243.15 | \-66.72 |
| 004 | Group 2 | 2024-03-25 | 1082.49 | na | na |
| 005 | Group 1 | 2024-03-27 | 1215.32 | 1497.63 | 282.31 |

What is needed here is more metadata.

In addition to documentation describing processes related to the above dataset, making use of it requires information about its structure and contents. In other words, a data dictionary or ReadMe file.

### Data Dictionaries

A **data dictionary** describes the elements of a collection of data. These documents may sound technical, but often can be as simple as a file containing the following:

1. A list of data elements in the dataset (e.g. variable names, column headers).  
2. A description of the properties of each element (e.g. data type, unit of measurement)  
3. The meaning of codes for categorical data within the dataset (e.g. “Group 1” vs “Group 2”)  
4. A description of the relationships between different elements within the dataset (i.e. how computed variables are created)  
5. A description of how missing data is handled.  
6. Any additional information or notes about the data needed to ensure its usability.

So for the dataset above, a simple data dictionary may look something like the following:

**Table 4.4. A Better Managed Dataset + A Data Dictionary**

| participant-id | group | date | rt-first | rt-second | rd-diff |
| ----: | ----: | ----: | ----: | ----: | ----: |
| 001 | Group 1 | 2024-03-15 | 1023.78 | 1891.42 | 867.64 |
| 002 | Group 2 | 2024-03-19 | 1147.21 | 1578.9 | 431.69 |
| 003 | Group 1 | 2024-03-21 | 1309.87 | 1243.15 | \-66.72 |
| 004 | Group 2 | 2024-03-25 | 1082.49 | na | na |
| 005 | Group 1 | 2024-03-27 | 1215.32 | 1497.63 | 282.31 |

| Variable Name | Human Readable Name | Units | Definition |
| :---- | :---- | :---- | :---- |
| participant-id | Participant ID number | This is nominal data | This is the ID number given to the participant to help ensure confidentiality. |
| group | Group | This is nominal data | This is the group the participant was assigned. These labels are used to blind the statistician to which is the control and experimental group. |
| date | Date of participation | This is a date | The day the participant enrolled in the study. All dates are in YYYY-MM-DD format. |
| rt-first | Average reaction time for the first set of trials | milliseconds | Missing data is coded as “na”. |
| rt-second | Average reaction time for the second set of trials | milliseconds | Missing data is coded as “na”. |
| rt-diff | The difference in average reaction time between the two sets of trials. | milliseconds. | This is a calculated variable (rt-second minus rt-first).  |

### ReadMe Files

But what if a dataset is more complicated than a single file?

A **ReadMe** can be thought of as a user guide that provides an explanation for how a set of files can be navigated and used. While a data dictionary should describe the structure and contents of a specific data file, a ReadMe provides a description of a larger dataset - which may include multiple files organized in multiple directories.

A readme is typically intended to be a human readable document, that lays out how a user can find and use the file or files they are looking for.

> **[Tool Highlight: ReadMe Template](https://docs.google.com/document/d/15lOyAQZIkex0aySqZ4giNlXJ-lcN00-NMWGd1wjX5IE/edit?tab=t.0)**
>
> ReadMe files are a form of research-related documentation that covers a complex dataset. 
>
> The best way for teams or individuals to use this template is use it as a starting point for systematizing their routine practices. This is just a format for getting started.
>
> Speaking of formats, this template uses minimal formatting so that it can be saved in any number of file types. By convention, ReadMe files are titled simply _readme.txt_ (or whatever file format), but it may be prudent to add the project’s name in there, for example _supportingdata-readme.txt._

## 4.5. Managing Documentation

**Figure 4.3.** below is an unfinished image of a crape myrtle \- often called the “lilac of the south” \- by Anne Kingsbury Wollstonecraft. Her manuscript, *Specimens of the Plants & Fruits of the Island of Cuba* (1827) was donated to the archives of Cornell University by one of her relatives, the great great grandfather of this guide’s author.

But, because references to the manuscript had incorrect metadata, its significance was not known until 2018 and Wollstonecraft’s family did not learn of its existence until 2024\.

|<img width="432" alt="Image" src="https://github.com/user-attachments/assets/e0853fd4-0bf4-4b43-a41b-7393a896b938" />|
| ----- |
| **Figure 4.3.** An unfinished image of the Largerstroemia (common crape myrtle) by Anne Kingsbury Wollstonecraft, from her documentation of Cuban flora.  The full, three volume manuscript has been preserved and is available for free online: Wollstonecraft, A.K. (1826) [*Specimens of the plants and fruits of the island of Cuba.*](https://catalog.hathitrust.org/Record/102498751) |

This example is an illustration of the importance of managing metadata properly. In the context of Good Data Management Practice, metadata describing scientific data should itself be considered scientific data. All of the same organizational and quality assurance practices should be applied.

It is very tempting to make assumptions when developing and preserving the type of documentation described in this chapter. The details of a procedure may seem too obvious to need recording, the variable names too clear. Maintaining good documentation does take time. But that time is an investment in preventing future headaches.

## Definitions of Key Terms

**Data Dictionary** - A document that describes the contents and structure of a dataset.

**Documentation** - Recorded information that is used to describe or explain something.

**Experimental Protocols** - A document, analagous to an SOP, that provides the precise steps needed to complete a research-related procedure.

**Good Documentation Practice** - A set of guidelines drawn from the pharmaceutical and manufactoring industries outlining how to maintain effective documentation.

**Lab Notebook** - A formal record of the research process. In the context of data management, lab notebooks are a form of contemporaneous documentation.

**Metadata** - Refers to information that facilitates the interpretation and/or use of research data. Can refer to formal metadata schemas (e.g. standardized ontologies) or to related documentation (data dictionaries, codebooks, protocols, etc).

**Metadata Schema** - A set of rules that are used to structure and describe metadata. A metadata schema defines metadata elements, what they mean, how they relate, and how they should be used.

**ReadMe** - A simple text document that lays out how a user can find and use the file they are looking for.

**Study Protocol** - A formal document that describes every aspect of a research project, including motivations, SOPs, data management, and planned statistical analyses.

## Further Reading

Bargaje, C. (2011). Good documentation practice in clinical research. *Perspectives in Clinical Research*, *2*(2), 59\. [https://doi.org/10.4103/2229-3485.80368](https://doi.org/10.4103/2229-3485.80368)

Kanare, H. M. (1985). *Writing the Laboratory Notebook*. American Chemical Society. Available online: [https://eric.ed.gov/?id=ED344734](https://eric.ed.gov/?id=ED344734)

## Footnotes

[^1]:  This quote was featured in “The Lives of Stars, the ninth episode of *Cosmos: A Personal Voyage.* This episode was first broadcast on November 25, 1980\.

[^2]:  Browse MeSH: https://www.ncbi.nlm.nih.gov/mesh/

[^3]:  See: Carp, J. (2012). Carp, J. (2012). On the Plurality of (Methodological) Worlds: Estimating the Analytic Flexibility of fMRI Experiments. *Frontiers in Neuroscience, 6*. [https://doi.org/10.3389/fnins.2012.00149](https://doi.org/10.3389/fnins.2012.00149)

[^4]: For example: Yang, P.-C., & Mahmood, T. (2012). Western blot: Technique, theory, and trouble shooting. *North American Journal of Medical Sciences*, *4*(9), 429\. [https://doi.org/10.4103/1947-2714.100998](https://doi.org/10.4103/1947-2714.100998)

[^5]:  The GCP Guidelines can be found via the [International Council for Harmonisation of Technical Requirements for Registration of Pharmaceuticals for Human Use (ICH)](https://www.ich.org/page/efficacy-guidelines), 

[^6]:  [NIH provides a variety of templates for writing protocols](https://grants.nih.gov/policy-and-compliance/policy-topics/clinical-trials/protocol-template)
