# Introduction

Should life scientists learn scripting languages?  Absolutely yes. Biology is increasingly becoming data intensive, and that means 
the researchers are spending more time parsing through large data files than working on the bench.  In the meanwhile, the computer 
languages and programming enviromnents are becoming easy to use and learn. R made statistical analysis and visualization straightforward, 
whereas python and PERL greatly simplified string processing and large-scale data analysis.

The current paradigm of biologists seeking help from the core facilities or specially-trained bioinformaticians for analysis of their data
is very inefficient. A recent paper discussing the work of bioinformatics core facilities wrote [1] -

"To give greater support to researchers, our centre set out to develop a series of standardized services. We documented the projects that we took on over 18 months. Forty-six of them required 151 data-analysis tasks. No project was identical, and we were surprised at how common one-off requests were (see .Routinely unique.). There were a few routine procedures that many people wanted, such as finding genes expressed in a disease. But 79% of techniques applied to fewer than 20% of the projects. In other words, most researchers came to the bioinformatics core seeking customized analysis, not a standardized package."

The above discussion reminded me of physics of the early 90s, when the theoretical physicists were not avid programmers.  When 
I joined graduate school, my professor did not know any programming and had to request his students to get all kinds of simple and 
complex calculations done.  That was frustrating for him and us, because we were busy with classes in the beginning and with our own 
research at the end. When his requests were different from our work, we had to switch mental context to write programs for him. That 
meant we could not invest as much time into exploring alternative ideas by playing with the program, as he could with full control
over the process.

What my professor did not realize was that programming was greatly simplified by tools like Matlab and Mathematica. Right after joining, 
I spent some time helping him learn Matlab, and he never had to ask anyone to do his analysis again. Moreover, Matlab was so easy that 
mostly he learned the language by himself through practicing. My role was to get him over the initial barrier and occasionally help 
him, when he got stuck.
 
Life scientists are at the same juncture today and can take care of much of their analysis on their own by learning R and some
other scripting language. This book and its associated training module are developed to help them get over the initial barrier.  This
book is written for PERL/python/GO together, but we also created equivalent notes for indivial languages available at the following
links. Moreover, we created a cloud-based environment, where they can practice  and online chat-based class for further training.
To get cloud account for practicing codes described in this book or to join our online chat-based class, please email pandora@homolog.us.


A scientific field is defined by the questions asked by its practitioners. Unless life scientists with experimental training start 
analyzing their own data, their whole field will get redefined by the computational scientists interested in different kind of 
questions.  For example, persons trained in computer science like to find problems, where they can show the mastery of their computer
skills. They may not think of ways or even ask questions that could be easily answered by additional experiments, because they may
lack access to experimental facilities or lack knowledge. One can see such change toward using excessive computation to solve all
problems happening in the field of human genetics, where researchers are proposing larger and larger genome sequencing problems 
(1,000, 10,000 or 100,000 human genomes) to answer increasingly trifling questions.

On the other hand, geneticists trained with working on individual genes cannot completely ignore the large-scale datasets available 
in the post-genomic era. Such exponential increase in data was a natural outcome of the completion of genome sequencing projects 
and rapid decrease over the last decade. Currently


 It  is less recognized is that the quality of individual observations  
continues to fall with this exponential rise of data.  For example, in the 90s, protein-protein interactions were measured
at the individual gene level, but each observation reported in papers were of high-quality. Since 2000, several groups reported 
measuring protein-protein interactions at the genome-wide scale, thus giving us thousands of interaction pairs.  It turned out that 
each interaction pair in their massive data sets were noisier than more careful individualized measurements of the earlier era. 
The same is true for all kinds of large-scale data sets published since the late 90s.

The biology of new era will consist of asking biological questions, but answering them through a combination of traditional experiments
and computational/statistical analysis of high-throughput datasets. This book prepares the biologists for the second task.

1. Core services: Reward bioinformaticians [http://www.nature.com/news/core-services-reward-bioinformaticians-1.17251#/]
