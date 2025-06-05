### Supporting Scientific Data | A Guide for Researchers

By John Borghi, PhD

This guide consists of a growing list of chapters, each covering a major topic in data management. These are complemented by a variety of explainers, checklists, and templates. In theory, these materials can all be read independently or in any order. 

This guide is generally tool agnostic. Several sentences may be devoted to a certain popular spreadsheet program, but otherwise the focus is largely on practices and strategies.

When complete, this guide will consist of approximately 10 chapters. Below are those that are complete enough for public dissemination. For the moment, even publicly available versions are quite drafty. So please don’t hesitate to reach out with comments, suggestions, questions, and recriminations.

| Chapter | Description |
| :---- | :---- |
| Understanding data management | This module defines data management in both technical and functional terms. |
| Defining research data | Data is more than just an individual file or set of measurements. This module details how to understand all of the components of data as situated within a research workflow. |

### 

### Before we get started in earnest…

These have their roots in an *Introduction to Research Data Management* workshop that is regularly taught at Stanford Medicine. That workshop is designed to be standalone, briskly paced, and largely didactic. While such a workshop can cover certain concepts and terms, managing scientific data effectively is not a process that can be covered or implemented just once. 

This guide aims to be *descriptive* \- outlining major concepts and practices related to data management in a way that is digestible to biomedical researchers. More prescriptive recommendations and requirements largely come from three sources: the institution where the research is taking place, organizations that provide research funding, and the research community itself. Policies and requirements from these entities will be discussed when relevant, but these requirements should not be an end to considerations related to data management, they should be a beginning. 

Data management should be an integral part of the day-to-day work of conducting research.

This guide also aims to provide information that is *actionable*, the following sections include a variety of exercises, thought experiments, tools, and links to additional resources to further develop data management and sharing-related practices. Over and over, these chapters will return to a concept creatively named Good Data Management Practice, but will remain largely tool agnostic. Though there may be mention of specific data-related tools and platforms, the focus will be on behaviors. 

Spoiler alert: There are more than a few worksheets and checklists ahead.

In reading, keep in mind that data management is not an all or nothing endeavor. Like many of the practices and concepts in biomedical research, strategies and practices related to data management exist along a continuum. One difficulty many researchers face when managing data is that there are always new tools, new requirements and expectations, and new norms. 

For these reasons, this guide is intended to be a living document, updated over time and in response to feedback. But, because we are all only human, it cannot possibly cover every strategy and practice related to managing the multifarious types of data involved in biomedical research.

Finally a few notes on terminology.

1. These modules follow a very inclusive definition of the term **researcher**. Professors, postdocs, and graduate students working on research projects are researchers, so are the lab techs, research assistants, staff, and other professionals who work alongside them.  
2. For somewhat related reasons, the term **data** is typically used as a singular mass noun (“data is”) rather than as a plural of datum (“data are”). 

This guide is built upon a broad and inclusive definition of what “counts” as both a researcher and as research data. Isolating an individual “datum” is often quite difficult. Making use of even a singular measurement from an instrument requires knowing some additional information about the processes and parameters used in its collection. For our purposes, a singular point of data is not typically a useful level of description. Neither is the spreadsheet that includes that point of data. Everything needed to reconstruct the workflow precedes a research finding “counts” as data. 

Sorry, not sorry.

Have fun\!?  
John

| ![][image1] | All chapters are licensed under a [Creative Commons Attribution-NonCommercial 4.0 Generic (CC BY-NC 4.0) License](https://creativecommons.org/licenses/by-nc/4.0/).  |
| :---: | :---- |

[image1]: <data:image/png;base64,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>