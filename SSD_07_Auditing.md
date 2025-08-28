# Monitoring and Auditing

| [Last Chapter - Sharing Data](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_06_Sharing) | [Back to the Table of Contents](https://johnborghi.github.io/Supporting_Scientific_Data/) | Next Chapter - Coming soon! |

## Chapter Summary

Data management is a continuous process. This section covers methods for ensuring that you (and your collaborators) are checking your work and staying ahead of evolving expectations and requirements.

This chapter is build around the principle that data management is a set of practices and strategies, not a set of tools.	

| [Principles of Good Data Management Practice](https://johnborghi.github.io/Supporting_Scientific_Data/supplements/SSD_good-dm-practice) | ["Good Enough" Practices in Data Management](https://johnborghi.github.io/Supporting_Scientific_Data/supplements/SSD_good-enough) |

|  | Key Points in this chapter |
| :---- | :---- |
| 1\. | To be maximally effective, data management must be implemented during the day-to-day course of a research project. Periodically, it is important to check your work. |
| 2\. | Data auditing involves conducting a comprehensive assessment of all data-related activities to ensure that they are being followed in line with a research group’s standard operating procedures. Auditing can also be used to identify gaps and areas where current SOPs are insufficient or no longer work. |
| 3\. | A data management audit can occur retrospectively or prospectively. A retrospective audit involves starting with the final publication describing a set of research findings and working backwards to see what data, documentation, and other materials remain accessible. A prospective data audit involves checking in on data management practices during the course of a research project. |

| **Supplementary Materials for this Chapter** |
| :---- |
|Way too many to list here. See **Table 7.2.** at the end of the chapter!|



## 7.1. Checking Your Work

When it comes to data management, it is important to check your work.

Thus far, this guide has covered some broad topics related to the management of research data and has provided some practical tips for maintaining Good Data Management Practice during the day-to-day work of doing science. Now it is time to take a step back, take a breath, and ensure everything is running as it should. 

The very first chapter introduced the following prompts as a way to start thinking about data management:

1. If another researcher were to ask for a copy of the data related to one of your projects, would you be able to easily find it and send it to them?  
     
2. If another researcher who works in the same field as you were to receive a copy of your data, would they be able to use it without asking you too many questions?  
     
3. Are you confident that you will be able to find and use the data from this project three years from now? How about ten years from now?

Hopefully these prompted some introspection and the intervening chapters have helped refine related practices and strategies. But, crucially, these questions are about outcomes. Like many aspects of data management, the idea is to understand the goal and work backwards to implement the activities needed to get there. What these questions do not touch on, at least directly, is how a research team actually goes about achieving their data management goals.

This chapter differs from the others in both length and structure. Affirmative responses to any or all of the questions posed above means that there is at least a semblance of a system in place for managing scientific data.That system may be a largely informal “way of doing things” or it could be a fully documented and refined set of protocols and standard operating procedures. While the latter is preferable of course, there is no singular system that is optimized or even appropriate for all research teams everywhere. But it is still vital that there is a system and that system is checked regularly. 

**Approach 1: Ensuring data quality**

There are several lenses through which a research team can view the act of checking that their data management system is working as intended. Probably the most immediately relevant is data quality.

Recall that the functional conception of data management introduced way back in the [introduction](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_01_introduction) covers practices and strategies designed to support the usability and quality of research data over time. The preceding chapters have largely focused on the “usability” aspect of data management. This chapter finally loops back to “quality”.

A common refrain in many areas of computing and scientific research is “garbage in, garbage out.[^1]” In research terms, this means If information or data is flawed, biased, or of low quality, then results based on that information or data are going to be flawed, biased, or of low quality. **Data quality** is a broad concept that refers to the degree to which a set of data is fit for its intended purpose. As shown in **Table 7.1**., this simple definition belies the complexity of this concept[^2]. A research team may be most concerned with *accuracy* and perhaps *timeliness*, but all five qualities are necessary for a dataset to be useful in a scientific research setting. 

**Table 7.1. Dimensions of Data Quality**

| Dimension | Definition |
| :---- | :---- |
| Accuracy | The data values are as close as possible to real values. |
| Completeness | All of the required data is present |
| Consistency | All data values are entered, formatted, and stored using a standardized set of rules. |
| Timeliness | The data is up-to-date. |
| Validity | The data is in the expected format, of the expected type, and within the expected range. |

Ensuring data is high quality involves several tightly related processes.

* **Quality control (QC)** refers to proactive efforts taken to ensure data quality.  
* **Quality assurance (QA)** refers to detection of problems that have already occurred.

This distinction is somewhat artificial, but **monitoring** ensures that the data management policies and procedures are in place and are being followed. Monitoring of data management activities should be routine and continuous. In contract, **auditing** is a process through which a team determines whether the monitoring program is operating as it should and that data-related policies are adequate and effective. Auditing often involves an outside party (i.e. individuals not on the research team). Because of the time and effort involved, audits are typically only done periodically.

One of the major complications for monitoring and auditing a team’s data management practices is that different types of data, different types of projects, and different research contexts will be associated with different expectations and requirements. 

More on this in a minute.

**Approach 2: We are all learning**

Though it can involve technical elements and tools, data management is ultimately a human process. A data management system is only as good as the researchers on a team remembering to name files appropriately, backup their data, and record the details of their workflow. 

“Best practices” in data management are also a moving target. Circumstances may change, necessitating a change in strategy. Research teams may turnover, necessitating training. Scientists are human, sometimes they make mistakes and forget things.

Much of this can be dealt with through thorough [planning](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_03_Planning) and even more thorough [documentation.](https://johnborghi.github.io/Supporting_Scientific_Data/SSD_04_documentation) But the work undertaken by most research teams \- especially in an academic research environment \- does not occur in a vacuum. To one degree or another, many members of such a team are learning on the job. It is not just students and other trainees learning how to do the job of scientific research. Everyone involved is constantly learning. This is part of the point.

This is not to say that anyone involved in a research project is exhibiting anything less than their absolute best efforts. But mistakes, if and when they happen, are learning opportunities. Discovering that a specific practice can be refined or needs to be changed is also a learning opportunity.

## 7.2. A Data Management Toolkit

There is not much more that can be presented didactically about monitoring and auditing data management practices. So class ends a little early today…

Just kidding.

Unlike other chapters where there are supplementary checklists and worksheets (and recipes?!) that complement the main text, this time around the checklists and worksheets are the main event. The whole point of monitoring and auditing data management practices is the implementation. 

To help research teams check their work in regards to data management, a suite of new materials are presented in **Table 7.2.**. From a thorough breakdown of the activities within a specific research project to a more general evaluation of a group’s data management practices, these tools cover data management at several different levels. Also included is a roles and responsibilities checklist, which is presented to help explicate who is responsible for a given data management-related activity and how often such activities are verified. All of these materials are intended to apply broadly, across many research areas. But one tool may be more useful to a research team than another. As always, they are intended as a starting point and can be used, adapted, and discarded as necessary.

**Using the toolkit:**

The materials in this toolkit are intended to allow a research team to check in on their data management practices in a way that works best for them. Team members are free to pick and choose which tools work best for them. The idea is less to demonstrate that a group is particularly "good" or "bad" at data management. But rather to equip researchers with ways of thinking about how they can support their data.

One final note: Depending on the circumstances monitoring and auditing data management practices may be a rather sensitive affair. Quality assurance and quality control are, of course, absolutely foundational to the scientific research enterprise. Checking to ensure that a practice is being implemented properly is not a critique of a research team or its members. Along the same lines, determining that a different practice may work better than an existing one is not a critique of the person who set up the data management system in the first place.  Remember, scientists are human, data management is a human process, and everyone is still learning.

**Table 7.2. A Toolkit for Monitoring and Auditing Data Management**

| Tool | Intended User | Description |
| :---- | :---- | :---- |
| [Data Management Checklist](https://docs.google.com/document/d/1cPtDmz50TyIsOA7BqMkMbNh20p1rzNsKFOk-k6biHZg/edit?usp=sharing) | An individual or research team who are thinking through how to integrate data management into their day-to-day practice. | Intended as the start of a conversation around data management, this checklist covers data management practices at a relatively high level. |
| [Prospective data audit](https://docs.google.com/document/d/1nEc6qUiaS8WERjAGjzCtpDfGGWz1ZlenfJPZv_pdvEc/edit?usp=sharing) (Forward track method) | An individual tasked with ensuring data is properly managed (i.e. a project PI, a lab manager, etc). | This checklist is intended to help a research team that their data management practices are implemented in line with their standard operating procedures. This form can also be used to demonstrate where additional discussion and training may be needed. |
| [Retrospective data audit](https://docs.google.com/document/d/1jZMPPYIRxgPD24DC6ON-c4JTImHuGcTZ-1m1VtaHPro/edit?usp=sharing) (Backwards track method) | Authors of a published scientific manuscript that present conclusions supported by research data. | This checklist is intended to help catalyze conversations within research teams about the accessibility of the data underlying their published manuscripts. Because it is designed to examine practices retrospectively, this exercise is not intended to be evaluative. But rather it will hopefully help teams evaluate their practices and advance them as needed or desired. [A short form is also available](https://docs.google.com/document/d/1os4P77RIWVdQGXPH73pmiDYvvaWR8LZ2vynppjUj3xY/edit?usp=sharing)|
| [Data Management Rubric](https://docs.google.com/document/d/112T8LLfNzkzZ7Ywtm5KPlevJrX03Gq7gR7ibFvvo6Lw/edit?usp=sharing) | Members of a research team who are interested in understanding how data management practices can be improved. | Data management is not a singular process, but rather an umbrella covering a wide variety of practices and strategies.  This rubric is designed to help teams understand where their practices are now, so they can chart a way towards where they want or need to be. |
| [Roles and Responsibilities Form](https://docs.google.com/document/d/1WQQxipEb3ER04-riJ-1eogAjO7neDIIpcMijbhMIOyM/edit?usp=sharing) | Members of a research team who are responsible for some aspect of data management. | This form allows a research team to make explicit the individual or individuals who will be responsible for carrying out different aspects of data management as well as the individual or individuals who will be responsible for verifying that these tasks are completed. This is meant to complement documented standard operating procedures (SOPs). |
| [Data Monitoring Form](https://docs.google.com/document/d/1RdQhIMpM2nrJV0atubpuW6-O31cqcG0OHP_jQWBE7i8/edit?usp=sharing) | An individual tasked with continuously monitoring that the data management practices within a research project are being implemented properly. | A checklist designed to help facilitate regular monitoring of data management practices within a given research effort. |

## Definitions of Key Terms

**Audit (Data Management)** \- An exercise designed to ensure that data management practices are being implemented properly. Is typically very involved and may not involve members of the research team.

**Data Quality** \- A broad concept that refers to the degree to which a set of data is fit for its intended purpose. Highly related to data management, but also includes issues more related to methodological rigor.

**Monitoring (Data Management)** \- A routine and continuous process designed to check that data management practices are being implemented according to standard operating procedures. Is typically less involved than a full audit and involves members of the research team.

**Quality Assurance/Quality Control (QA/QC)** \- Retrospective and prospective efforts to assure data quality. The terms are often used interchangeably.


