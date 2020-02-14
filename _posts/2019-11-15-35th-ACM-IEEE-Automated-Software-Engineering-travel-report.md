---
layout: post
title: "Explore the conference: 35th ACM/IEEE Automated Software Engineering 2019 Travel Report"
author: "Haemin Ryu"
---

# About ASE 2019 
I participated the 34th IEEE/ACM International Conference on Automated Software Engineering (ASE 2019), which was located at San Diego from November 11 to 15, 2019.
Automated Software Engineering is the premier research forum for automated software engineering and it is a top-tier ACM conference in the areas of Software Engineering. 
Each year, it brings together researchers and practitioners from academia and industry to discuss foundations, techniques, and tools for automating the analysis, design, implementation, testing, and maintenance of large software systems.
This is the first time I'm attending ACM Conference, and interesting to know that
This year, ASE has 91 regular paper submissions, and 23 presentations from papers in the top software engineering journals, 36 demos of cutting-edge tools for automated software engineering, and 14 student papers compete to participate in the ACM Student Research Competition Grand Finals.

# Before attending the ASE 2019 conference

link: https://docs.google.com/presentation/d/1fOrNZoqKhigadi4jadvt4Nsc_wKOqVVT_tlyVR5s_Kc/edit?usp=sharing 

# After attending the ASE 2019 conference

## Day-1 (Mon 11 Nov):

The workshop I attended on day-1 were about mobile app analysis (A-Mobile) aims at bringing together international researchers and practitioners in the field of mobile app analysis to present and discuss emerging advanced techniques.
One of the interesting papers was the following one about Automated Support for Testing and Maintenance of Mobile Applications by Mattia Fazzini (University of Minnesota).
This paper talked about Automated Support for Testing and Maintenance of Mobile Applications. 

Another paper I was interested in was "SeMA: A Design Methodology for Building Secure Android Apps" by Joydeep Mitra, Venkatesh-Prasad Ranganath.


## Day-2 (Tue 12 Nov):

Keynote: "Re-engineering Software Engineering for a Data-centric World" 
by Miryung Kim _ University of California, Los Angeles

<Summary of the Keynote> 
Confluence: Interdisciplinary Thinking, Data Analytics 
New reflection of Data Analytics(SE4DA)
= underserved. 
There is a huge opportunity for data analytics 
AI bias
 
Data analytics are in high demand, yet … 
Bugs are huge problems in data analytics: misleading, predictably inaccurate. 
ex) A self driving car killed a women. 
 
SE4DA is under-investigated, only 13 papers to enhance the DA. 
 
Outline: Making a Case for SE4DA
data -centric SW development
Traditional process vs data-centric
Debugging and testing for big data analytics
Open problems
 
Data Scientist? Clustering algorithms. Based on relative time spent in activities -> 9 distinct categories. 
<Distinct categories>
Data Shaper
Platform Builder
Data Analyzer
 
Challenges: To ensure correctness
 
Traditional SW vs Data-centric SW
Big Data analytics dev
Developing locally test locally execute the job on the cloud and later job crashes repeat this process
 
1.Data is huge
2. Writing test is hard
3.Failure 
4. System stack is complex with little visibility. 
 
 
Debugging & Testing for big data analytics
Insights from Debugging and Testing for Apache Spark 
How execution is actually done 
Modifying s tunyimr -> no trace
Abstraction 
 
Re-think a traditional 
 
BigDebug
Titian
BigShift: debugging 66x faster than delta debugging
 
Why is Testing Big Data Analytics Challenging? 
=> Testing time!!
=> Symbolic execution

BigTest: White-Box Testing of Big Data Analytics

Test Size Reduction 
: You don’t need to test it all 

Open problems
Accelerating Data-Centrice Dev
2019: Collaborate with systems, ML, DV to design tool
Co-developed with runtimes framework

How to define a bug based on the properties of both data and code? 
How to repair 
Performance debugging is a pain point 
StackOverFlow: Performance is the biggest problem. 
	Details : related to I/O, cluster

Performance debugging requires visibility of system stack, code, and data. 
How to estimate performance based on data size? 
How to optimize query performance using a cost?
How to debug computation and data skews? 
How to identify the cause of bottlenecks? 

We must relax the strict notion of incorrect behavior and the root cause. 
Specify oracles:	
Metamorphic Testing: DeepTest, DeepCancolic, DeepHunter
	Quentify importance
	LIME,Lamp … 


## Day-3 (Wed 13 Nov):

Keynote: "The Human Dimension of Cloud Computing" (Wed 13 Nov) 
by Yuanyuan Zhou _ University of California, San Diego

<Summary of Keynote> 

Cloud is Used in Almost Every Enterprise.
Cloud-Powered AI & Advanced Data Processing 
Sysadmins are getting scared 
Sysdamin’s errors have caused many failures 
Configuration Errors in Google 
Sysadmin error is also a major security risk 
Our Project 
Understanding real world sysadmin errors 
Real world security 
Address it in a more fundamental way 


Why is configuration so damn hard? 
Too many knobs!! 
Configuration knobs are seldom removed. 
Do sysadmins really need so many knobs? 
	
Implication 
	We have given our sysadmins too many knobs!! 
What is the cost of too many knobs? 
Real-world example of incorrect defaults 
Root cause 
Cloudera : “One of the most common problems from our users”
How much can we simplify? 
Shall we offer more choices in setting knobs? 
Similar findings! 
Guidelines for simplifying configuration 

How Cloud Configuration Missteps Lead to Data Breaches 

Our Next Study
How sysadmins configure access-control setting? 
Particularly, how to handle access deny cases
Obstacles to fix access permission correctly 
What information/tools are missing? 

Common insecure fixes to access-denied issues 
Disable protection
Grant all priv
Add permission. 

Common security misconfigurations

Resolution through trial and error 
Distributions of useless fixes 

Deficiency of existing log messages
Example: too general notifications 

Should we tame the beast before it is uncontrollable? 


