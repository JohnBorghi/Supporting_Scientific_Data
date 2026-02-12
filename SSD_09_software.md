
## 9.1. What is software?

The year is 1925. Ronald Fisher is a geneticist and statistician[^1] working at Rothamsted Experimental Station, an agricultural research institute located in the English countryside. A plethora of long term experiments give Fisher a bumper crop of data to analyze. However, though the quantity of data is high, sample sizes are low. One study, examining the effects of rainfall on the growth of wheat, incorporates data from just thirteen plots of land.

Concerned with the generalizability of his work, Fisher synthesizes several recent advances in “small sample statistics” into a framework known as “significance testing”. He expands the utility of Student’s t-test - a statistical device initially developed by William Sealy Gosset to monitor the quality of beer - and develops a complementary test known as the Analysis of Variance (ANOVA). To ensure these innovations are accessible to the research community beyond Rothamsted, Fisher publishes an influential volume [Statistical Methods for Research Workers](https://archive.org/details/in.ernet.dli.2015.205971).

Central to the book, and significance testing more generally, is the null hypothesis - the position that there is no significant difference between groups of data. The results of statistical tests like t-tests and ANOVAs indicate the likelihood of observing a pattern of results when the null hypothesis is true. In quantitative terms, this likelihood is expressed as a p-value. In Statistical Methods for Research Workers, Fisher introduces an informal criterion for rejecting the null hypothesis: p < 0.05. These developments only grow in influence with the publication of [The Design of Experiments](https://archive.org/details/in.ernet.dli.2015.502684).

This early history of statistical research methods intersected with the development of modern computing. At Rothamsted, Fisher made extensive use of “The Millionaire”, the first commercially successful calculating machine. In the subsequent decades, work at Rothamsted would continue to leverage advances in computational technology. By the 1960s, researchers at the institute had developed thousands of miles of paper tape - for calculating regressions, multivariate analyses, and conducting all manner of other statistical operations. In modern parlance, we would call this software.

By 1968, the software at Rothamsted was compiled into the statistical software package Genstat. Nearly simultaneously, teams at the North Carolina State University and University of Chicago developed SAS and SPSS. Researchers continue to use these tools - and so, so many others - as part of their work. Software, like data, is also an important product of the research process in and of itself. 

For the purposes of Good Data Management Practice, **software** can be very broadly defined as an object that instructions for a computer. In a research setting, such objects take several forms
1. **Code** - Instructions that implement specific processes, analyses, or other workflows. Code is written in languages like R, Python, Matlab, and C++.
2. **Packages** Collections of written code that - together - provide computational functionality that can be incorporated into other software. Also called _libraries_ or _toolboxes_, examples include the tidyverse packages, NumPy, and SciPy, and Tensorflow.
3. **Applications** - A form of software that is packaged and developed to be run easily by end users. Tools like SPSS, SAS, and Excel are examples of applications.

As usual, the line between these is often fuzzy. For the most part, the most useful distintion is between software that researchers write as part of their work and software that researchers use as part of their work.

### Software is like data

Especially under a workflow-based definition of scientific data, software can be categorized as a form of data. Software can be the tool through which data is collected, recorded, and analyzed. It is also metadata. As best illustrated by research-related code, software represents the precise steps implemented during part of the research process. As such, software is an essential element of establishing data provenance. We will get into the how later in this chapter, but, like data, research-related software needs to be thoughtfully managed and disseminated.

### Software is not like data

However, even under this guide's extremely broad definition of scientific data, software is something of a different ballgame. This _is_ a tremendous oversimplification but data is while software _does_. A set of research data is not necessarily a static object but, in general, data is something we act upon while software performs a particular function (e.g. analyzing a dataset). Software is executable. Software also has a different set of needs than data and its proper management requires different skills and vocabulary.

## 9.2. Why does software matter?

Reproducibility – Others must be able to rerun analyses.

Transparency – reviewers and readers can inspect methods.

Reuse – code can be adapted, extended, or validated.

Preservation – ensuring future access even after projects end.

Policy Compliance

## 9.3. Development and documentation

## 9.4. It works on my machine?

## 9.5. Archiviving, Preservation, and Sharing

[1]: Fisher leaves a complex legacy in the history of science. His work made substantial contributions to concepts and methods that are still in broad use today. But this must be viewed in light of his enthusiastic support for eugenics.










