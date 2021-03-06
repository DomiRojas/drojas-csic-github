Preface

This introduction to R is derived from an original set of notes describing the S and S-Plus
environments written in 1990–2 by Bill Venables and David M. Smith when at the University
of Adelaide. We have made a number of small changes to reflect differences between the R and
S programs, and expanded some of the material.

1 Introduction and preliminaries

1.1 The R environment

R is an integrated suite of software facilities for data manipulation, calculation and graphical
display. Among other things it has
 an effective data handling and storage facility,
 a suite of operators for calculations on arrays, in particular matrices,
 a large, coherent, integrated collection of intermediate tools for data analysis,
 graphical facilities for data analysis and display either directly at the computer or on hardcopy,
and
 a well developed, simple and effective programming language (called ‘S’) which includes
conditionals, loops, user defined recursive functions and input and output facilities. (Indeed
most of the system supplied functions are themselves written in the S language.)
The term “environment” is intended to characterize it as a fully planned and coherent system,
rather than an incremental accretion of very specific and inflexible tools, as is frequently the
case with other data analysis software.
R is very much a vehicle for newly developing methods of interactive data analysis. It has
developed rapidly, and has been extended by a large collection of packages. However, most
programs written in R are essentially ephemeral, written for a single piece of data analysis.

1.2 Related software and documentation

R can be regarded as an implementation of the S language which was developed at Bell Laboratories
by Rick Becker, John Chambers and Allan Wilks, and also forms the basis of the S-Plus
systems.
The evolution of the S language is characterized by four books by John Chambers and
coauthors. For R, the basic reference is The New S Language: A Programming Environment
for Data Analysis and Graphics by Richard A. Becker, John M. Chambers and Allan R. Wilks.
The new features of the 1991 release of S are covered in Statistical Models in S edited by John
M. Chambers and Trevor J. Hastie. The formal methods and classes of the methods package are
based on those described in Programming with Data by John M. Chambers. See Appendix F
[References], page 96, for precise references.
There are now a number of books which describe how to use R for data analysis and statistics,
and documentation for S/S-Plus can typically be used with R, keeping the differences between
the S implementations in mind. See Section “What documentation exists for R?” in The R
statistical system FAQ.

1.3 R and statistics

Our introduction to the R environment did not mention statistics, yet many people use R as a
statistics system. We prefer to think of it of an environment within which many classical and
modern statistical techniques have been implemented. A few of these are built into the base R
environment, but many are supplied as packages. There are about 25 packages supplied with
R (called “standard” and “recommended” packages) and many more are available through the
CRAN family of Internet sites (via https://CRAN.R-project.org) and elsewhere. More details
on packages are given later (see Chapter 13 [Packages], page 77).
Most classical statistics and much of the latest methodology is available for use with R, but
users may need to be prepared to do a little work to find it.
There is an important difference in philosophy between S (and hence R) and the other
main statistical systems. In S a statistical analysis is normally done as a series of steps, with
intermediate results being stored in objects. Thus whereas SAS and SPSS will give copious
output from a regression or discriminant analysis, R will give minimal output and store the
results in a fit object for subsequent interrogation by further R functions.
