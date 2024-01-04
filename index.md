## About 

I'm an assistant professor of math at [Flathead Valley Community College](https://www.fvcc.edu). I primarily teach intro statistics and the courses feeding into this class, but my background is in low-dimensional topology. Back in the day I thought about 3-manifolds and the character varieties thereof, but lately I've pivoted towards thinking about data analysis/science and machine learning.  

In 2022 I started working part-time as a data analyst for FVCC. This role involves performing in-depth statistical analyses, developing and maintaining Tableau dashboards, ETL and automation projects related to IR and IT, and fulfilling adhoc data requests. I interact with a wide variety of stakeholders across campus, from faculty to the financial aid and business offices to the executive team, and leverage my experience as en educator to clearly communicate technical results to all parties.

To see more about my background, check out my

- [Resume](./resume/resume.pdf) and 

- An older CV



### Teaching resources

- [STAT216](./stat216): Find here a playlist of videos I made for FVCC's online intro stats class, notes on using R for basic inferential statistics, 

- [M115](./m115)

### Projects

#### For FVCC

- *Degree Audit Program:* I built a tool that allows advisers to quickly view a student's progress on *any* program at FVCC in any relevant catalog year. I used the data underlying this program to identify roughly 700 former FVCC students who had completed at least 75\% of some program, many of whom had fulfilled all program requirements without graduating. Targeted recruiting to this group of students will increase FVCC enrollment and graduation rates.   This project proceeded in four main steps:

    - ETL: Scrape the [FVCC Catalog](https://catalog.fvcc.edu/) with Acalog's API, parse the resulting XML and tidy the resulting program requirement dataset, then write the dataset to an FVCC SQL Server. 
    
    -  Join all student course records to all program requirements. 
    
    - Optimize course assignment. Each course can only satisfy one program requirement, but some courses can satisfy multiple program requirements. I maximize the number of requirements met in each program by thinking of course assignment as a network flow from student courses to program requirements and calculating a maximum flow. 
    
    - Build a Tableau dashboard to display the results  
    
- *Enrollment Dashboard*

- *Math and Chemistry Placement Test Analysis* 

- *No Holding Back Analysis*

#### Contract 

- *Kalispell SD5 5 and 10 year enrollment forecasting*

- *Glacier High School **Ascent Program** efficacy analysis*

#### Personal

Below you'll find links to a few semi-silly personal projects. The less silly a project sounds, the higher probability it has of being incomplete. 

- NW Montana avalanche forecast generator

- [Montana scratch lotto web-scrape](https://github.com/ckaterba/ScratchLottoScrape)

- [Winter sports heat map](../DDP_projects/docs/DDP_project_1_ski_heatmap.html)

- [Naive Wordle solver](./wordle): Created when the game Wordle first started making waves. This solver simply makes a random guess for the first word, trims the dictionary using information from the first guess, then randomly picks another word and repeates until it guesses correctly. 

- [A planet with a moon orbiting a star](https://www.shadertoy.com/view/NdGyWh): Simple ray tracing animation created in ShaderToy.


#### Math

- [Ideal points of character varieties, algebraic non-integral representations, and undetected closed essential surfaces in 3-manifolds](https://arxiv.org/abs/1808.02535). Link to pre-print of a paper published in the Proceedings of the AMS. Joint work with Alex Casella and Stephan Tillmann.

- [Modules, fields of definition, and the Culler--Shalen norm](https://arxiv.org/abs/1805.04585). Link to pre-print of a paper submitted to Algebraic and Geometric Topology. 

- Indra's Pearls Undergrad research project, include image and link to some code

- Twist-knot intersections in the character variety of the Whitehead link. Project in progress with Tim Morris. [Link to some computations in Sage](https://github.com/ckaterba/Twist_Knot_CharVar_Intersection/blob/main/twistIntExploration.ipynb).



