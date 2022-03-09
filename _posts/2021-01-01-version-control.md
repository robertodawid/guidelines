---
layout: post
title:  "Version Control"
date:   2021-01-01
comments: true
author: Will Usher
category: practice
tags: ubuntu retrievability repeatability reusability reconstructability auditability
---

Version Control Systems (VCS), such as Git, Mecurial and Subversion
provide the ability to record a history of changes to source code, data,
 or other text-based material,
 and then switch between these points in the history
 or view the differences between them.
 In short, version control provides "infinite levels of undo".

Version control enables collaborative workflows
in either a centralised or distributed fashion,
which can effectively support scientific work.
Because each change to tracked content is recorded,
conflicts between changes can be resolved in a systematic fashion.
This gives collaborators the freedom to make changes as they want,
and then merge their changes when they are ready.

The use of version control supports reproducibility and transparency
through the consistent and structured workflow necessary
for working with a VCS.
For example, messages associated with changes to the code ["commits"]
provide a running commentary on the development of the work itself.
Version control allows entire repositories to be easily shared,
facilitating the publishing of the work online,
through websites such as Github and Gitlab [37].

# Applying version control to software

Version Control is now seen as a cornerstone of reproducible computational research.
Recognising that even small changes to computer code
can have large unintended consequences
on the output of scientific software,
then version control provides a structured and convenient means
to record which version of scientific software was used for a study.

The ability to easily switch between code versions
supports systematic approaches to debugging,
and the reproduction of results from different points in the project
[(Sandve et al., 2013)][3].

# Applying version control to data

Most version control systems are designed for management of source code,
which is text-based.

If data is stored as text,
for example in comma-separated value files (csv),
or as a [Frictionless Data Package][4],
then that data can be placed under version control.
This provides all the benefits listed above,
in terms of enabling collaboration
and providing a systematic process for updating and versioning the data.

There are also number of tools that allow binary data to be placed
under version control including [Git-LFS][5], which replaces large files with text pointers to the files stored on a server,
and [DVC][6],
which was built for data scientists and machine learning
projects.

# Applying version control to other material

This material is derived from the [CCG review of good enough practices][1] which is released under a [CC-BY 4.0 license][2].

[1]: https://doi.org/10.5281/zenodo.5911546 "Usher, William, Beltramo, Agnese, Gardumi, Francesco, Martin, Viktoria, & Petrarulo, Luca. (2022). CCG Platform - Body of Knowledge: Review of Good Practice (1.3). Zenodo. https://doi.org/10.5281/zenodo.5911546"

[2]: https://creativecommons.org/licenses/by/4.0/legalcode

[3]: https://doi.org/10.1371/journal.pcbi.1003285 "G. K. Sandve, A. Nekrutenko, J. Taylor, and E. Hovig, ‘Ten Simple Rules for Reproducible Computational Research’, PLOS Computational Biology, vol. 9, no. 10, p. e1003285, Oct. 2013, doi: 10.1371/journal.pcbi.1003285."

[4]: https://specs.frictionlessdata.io/data-package/ "Frictionless Data Package"

[5]: https://git-lfs.github.com/ "Git Large-File-System"

[6]: https://dvc.org/ "DVC"