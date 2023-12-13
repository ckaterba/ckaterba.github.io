## About 

I'm an assistant professor of math at [Flathead Valley Community College](https://www.fvcc.edu). I primarily teach intro statistics and the courses feeding into this class, but my background is in low-dimensional topology. Back in the day I thought about 3-manifolds and the character varieties thereof, but lately I've pivoted towards thinking about data analysis/science and machine learning.  

In 2022 I started working part-time as a data analyst for FVCC. This role involves fulfilling ad-hoc data requests for stake holders across campus, developing and maintaining Tableau dashboards to increase access to data, numerous ETL projects related to IR and IT, and 

### Teaching resources

- [STAT216](./stat216)

- [M115](./m115)

### Professional things

- Resume

- Old CV

### Projects

#### Data 

**FVCC**

- *Degree Audit Program:* I built a tool that allows advisors to quickly view a student's progress on *any* program at FVCC in any relevant catalog year. I used the data underlying this program to identify roughly 700 former FVCC students who had completed at least 75\% of some program, many of whom had fulfilled all program requirements without graduating. Targeted recruiting to this group of students will increase FVCC enrollment and graduation rates.   This project proceeded in four main steps:

    - ETL: Scrape the [FVCC Catalog](https://catalog.fvcc.edu/) with Acalog's API, parse the resulting XML and tidy the resulting program requirement dataset, then write the dataset to an FVCC SQL Server. 
    
    -  Join all student course records to all program requirements. 
    
    - Optimize course assignment. Each course can only satisfy one program requirement, but some courses can satisfy multiple program requirements. I maximize the number of requirements met in each program by thinking of course assignment as a network flow from student courses to program requirements and calculating a maximum flow. 
    
    - Build a Tableau dashboard to display the results. 


- *Enrollment Dashboard*

- 

**Contract**

**Personal**

- NW Montana avalanche forecast generator [work in progress]

- Montana scratch lotto web-scrape and analysis

- Winter sports heat map

- Naive Wordle solver 

#### Math

- [Ideal points of character varieties, algebraic non-integral representations, and undetected closed essential surfaces in 3-manifolds](https://arxiv.org/abs/1808.02535). Link to pre-print of a paper published in the Proceedings of the AMS. Joint work with Alex Casella and Stephan Tillmann.

- [Modules, fields of definition, and the Culler--Shalen norm](https://arxiv.org/abs/1805.04585). Link to pre-print of a paper submitted to Algebraic and Geometric Topology. 

- Twist-knot intersection github, paper in progress 

- Indra's Pearls github

- ray tracing in ShaderToy





