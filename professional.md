## Select Data Projects

### At FVCC

- *Degree Audit Program:* I built a tool that allows advisers to quickly view a student's progress on *any* program at FVCC in any relevant catalog year. I used the data underlying this program to identify roughly 700 former FVCC students who had completed at least 75\% of some program, many of whom had fulfilled all program requirements without graduating. Targeted recruiting to this group of students will increase FVCC enrollment and graduation rates.   This project proceeded in four main steps:

    - ETL: Scrape the [FVCC Catalog](https://catalog.fvcc.edu/) with Acalog's API, parse the resulting XML and tidy the resulting program requirement dataset, then write the dataset to an FVCC SQL Server. 
    
    -  Join all student course records to all program requirements. 
    
    - Optimize course assignment. Each course can only satisfy one program requirement, but some courses can satisfy multiple program requirements. I maximize the number of requirements met in each program by thinking of course assignment as a network flow from student courses to program requirements and calculating a maximum flow. 
    
    - Build a Tableau dashboard to display the results  
    
- *Enrollment Dashboard*

- *Math and Chemistry Placement Test Analysis* 

- *No Holding Back Analysis*

### Contract work

- *Kalispell SD5 5 and 10 year enrollment forecasting*

- *Glacier High School **Ascent Program** efficacy analysis*