# Social Media Analysis
<i> This projects uses social media in an attempt to find HR insights. </i>
(It's still very exploratory right now.)

Organizations  have employees working in different specializations.  Creating a job description for each role helps organize the workforce.  This is often decided based on what the employee is doing (marketing, engineering, etc.) and their level (manager, director, etc.).  A good job descriptions can be used as the foundation of organization design planning, compensation strategies, and recruiting processes. 

This exercise analyzes public job descriptions from multiple organizations to find similarities and differences.  
- Since the Human Resources division is generally responsible for writing the job descriptions, this exercise began by focusing on job descriptions of Human Resources positions (since HR should have the best understand about roles on their own team).  
- Higher level positions often get more attention, so this project focused on the top level HR position irrespective of its title (Head of People, Chief People Officer, Global Head of Talent Management, etc.).  
- Remote job descriptions were chosen to limit any bias in a specific geography, though all job descriptions were posted in English.  
- Companies generally had headcounts over 50 workers (since below that headcount, this role is often an individual contributor) and under 500 workers (since above that headcount, role are often recruited through an employment agency, not posted publicly online).   
- The job descriptions were taking in the 2nd, 3rd, and 4th quarter of 2022 to avoid influences of major COVID lock-downs or pre-COVID norms.

Each job description had its text manually divided into different categories: 
- AboutRole - description of what the role is responsible for, what the day-to-day is, where it fits into the organization structure
- AboutCompany - information on the type of organization that is hiring the role
- Requirements - what traits the candidate needs to be hired
- NiceToHave - preferred, but not mandatory traits for the candidate
- Benefits - what the organizations provides to the candidate (healthcare, time off, etc.)
- Diversity - text discussing the organization's commitment to fair hiring practices regarding Diversity, Equity, Inclusion, and Belonging or an Equal Opportunity statement (often added at the end of the job description) 

Although the manual process of breaking up the text into buckets was imperfect, it should help better identify the context of the word. If the word "Compensation" used in the requirements section, is probably asking the if the candidate has experience in managing compensation plans.  If the word “Compensation” is used in the Benefits or Diversity section, it is probably talking about the compensation that will be paid to the candidate or the fairness in pay, respectively.

# Top Words in “Requirements” Section for Head of HR Jobs:

We can see some common traits across job descriptions when just looking at the “requirements” section of the posting.  Here all stop-words (like “the” or “a”) are removed, in addition to many common HR words (like “days” or  “company”) that would not be useful in the analysis.  

More work needs to be done to combine similar phrases like “Talent Acquisition” and “Recruiting”, which will move them higher on the word count list.

<kbd><img src="https://github.com/LookHere/SocialMediaAnalysis/blob/main/Files/Images/MostCommonWords.jpeg" width=100% height=100%></kbd>


# Sentiment Analysis 

Human Resources as a profession is known to be friendly.  By passing the job descriptions through a rudimentary sentiment analysis we can see which postings use the most positive words.  The format of job descriptions make them easier to run sentiment analysis on since they generally don’t include things like sarcasm and innuendo, which are challenging for the analysis.

At first glance, it’s clear that the longer postings had higher positive scores in total.

<kbd><img src="https://github.com/LookHere/SocialMediaAnalysis/blob/main/Files/Images/Positivity.jpeg" width=100% height=100%></kbd>

But if we divide the positivity score by the number of characters, we can see that the average positivity by character is actually higher for the shorter job descriptions.  The trend for longer job descriptions to have fewer positive words per character is one of the many reasons we should try to keep our job descriptions short and to the point.  We want the candidate to have constant positive reinforcement through the entire time they are interacting with our brand.

<kbd><img src="https://github.com/LookHere/SocialMediaAnalysis/blob/main/Files/Images/PositivityByCharacter.jpeg " width=100% height=100%></kbd>


# Project Roadmap
- [x] find a population of job descriptions
- [x] break up job descriptions into buckets
- [x] find the most common words in those buckets
- [x] create a wordcloud to visually display the most common words
- [x] perform sentiment analysis to see which roles have the most positive phrasing
- [ ] develop a way to merges similar terms (like "Recruiting" and "Talent Acquisition") 
- [ ] compare Head of HR to similar roles, like Head of Finance
- [ ] understand which roles use “years of experience” and what the year correlate to
- [ ] see which benefits organizations are using to attract candidates
- [ ] analyze DEIB (Diversity, Equity, Inclusion, and Belonging) statements to see outward facing cultural values
- [ ] develop a system to automatically scrape websites to pull in the job descriptions
- [ ] develop a system to automatically divides the data into the right buckets (or at least help speed up that process)

<kbd><img src="https://github.com/LookHere/SocialMediaAnalysis/blob/main/Files/Images/HeadOfHRWordCloud.jpeg" width=100% height=100%></kbd>
