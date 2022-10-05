# SocialMediaAnalysis
<i> This projects uses social media in an attempt to find HR insights. </i>

Organizations can have people working in different specializations.  Creating a job description for each role helps organize the workforce.  This is often decided based on what the employee is doing (marketing, engineering, etc.) and their level (manager, director, etc.).  A good job descriptions can be used as the foundation of organization design, compensation, and recruiting processes. 

This exercise analyzes public job descriptions from multiple organizations to find similarities and differences.  
- Since the Human Resources division is generally responsible for writing the job descriptions, this exercise began by focusing on job descriptions of Human Resources positions (since HR should understand roles on their own team the most).  
- Higher level positions often get more focus, so this project focused on the top level HR position irrespective of its title (Head of People, Chief People Officer, Global Head of Talent Management, etc.).  
- Remote job descriptions were chosen to limit any bias in a specific geography.  
- Companies generally had headcounts over 50 workers (since below that headcount, this role is often an individual contributor) and under 500 workers (since above that headcount, role are often recruited through an employment agency, not posted publicly online).   
- The job descriptions were taking in the 2nd, 3rd, and 4th quarter of 2022 to avoid influences of major COVID lock-downs or pre-COVID norms.

Each job description had its text manually divided into different categories: 
- AboutRole - description of what the role is responsible for, what the day-to-day is, where it fits into the organization structure
- AboutCompany - information on the type of organization that is hiring the role
- Requirements - what traits the candidate needs to be hired
- NiceToHave - preferred, but not mandatory traits for the candidate
- Benefits - what the organizations provides to the candidate (healthcare, time off, etc.)
- Diversity - text (often at the end of the job description) discussing the organizations commitment to fair hiring practices regarding Diversity, Equity, Inclusion, and Belonging or an Equal Opportunity statement

Although the manual process of breaking up the text into buckets was imperfect, it should help better identify the context of the word. If the word "Compensation" used in the requirements section, is probably asking the if the candidate has experience in managing compensation plans.  If the word “Compensation” is used in the Benefits or Diversity section, it is probably talking about the compensation that will be paid to this job or the fairness in pay, respectively.

# Top Words In “Requirements” For Top Level HR Roles:

<kbd><img src="https://github.com/LookHere/SocialMediaAnalysis/blob/main/Files/Images/MostCommonWords.jpeg" width=100% height=100%></kbd>

## Project Roadmap
- [x] find a population of job descriptions
- [x] break up job descriptions into buckets
- [x] find the most common words in those buckets
- [x] create a wordcloud to visually display the most common words
- [ ] build something that merges similar terms (Recruiting and Talent Acquisition) 
- [ ] compare this to similar roles, like Head of Finance
- [ ] understand which roles use “years of experience” and if the years are correlated to anything
- [ ] see which benefits organizations are using to attract candidates
- [ ] analyze DEIB (Diversity, Equity, Inclusion, and Belonging) statements to see outward facing cultural changes
- [ ] develop a system to automatically pull this data
- [ ] develop a system to automatically break the data into the right buckets (or at least help speed up that process)

<kbd><img src="https://github.com/LookHere/SocialMediaAnalysis/blob/main/Files/Images/HeadOfHRWordCloud.jpeg" width=100% height=100%></kbd>
