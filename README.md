# portfolio
repo for code that shows progress in using software tools

# first python program; written in python 2.6
EnrollReportProcessing.py is a script that cleans up college generated report.  Unfortunately, these auto-generated reports are designed to be read in excel and so they have row headings embedded throughout. Also, some of the column titles are merged across two rows, and some columns are actually two merged variables.  This script (or series of scripts) filters out the unnecessary rows and splits data into tidy csv tables (see: [Wickham, H. (2014). Tidy Data. Journal of Statistical Software, 59(10), 1 - 23. doi:http://dx.doi.org/10.18637/jss.v059.i10]).  

For example. An auto-generated report looks like this:
```
Spring 18 : 7/14/2018 6:43:48 PM,,,,,,,,,,,,,,,,,,
,,,,,,,,,,,,,,,,,,
Report Title: All Classes,,,,,,,,,,,,,,,,,,
,,,,,,,,,,,,,,,,,,
Non-Clustered Classes:,,,,,,,,,,,,,,,,,,
Item,Course ID,Title,CR,Days,Class Time,,Room,Instructor,Enrolled,,,Wait,FTES,,Budget,,,
,,,,,Start,End,,,,,,List,TOTAL,STATE,PRG-ORG,,AU,
1811,ABE 031 01,ABE MATH LEVEL 3,5,DAILY,11:00 AM,11:50 AM,IB 3330,Jlemley,16,/,28,0,5.3,5.3,11,3L01,AA,
1839,ABE 031 11,ABE MATH LEVEL 3,5,DAILY,11:00 AM,11:50 AM,IB 3309,Cancel 03/01,0,/,0,0,0,0,,,AA,
1831,ABE 040 01,ABE/HS 21 LANG ARTS,5,DAILY,9:00 AM,9:50 AM,IB 3330,Jlemley,8,/,28,0,2.7,2.7,,,AF,

[...]

```

The script yields this:
```
Spring 2018,North,1811,ABE 031 01,ABE MATH LEVEL 3,5,DAILY,11:00 AM,11:50 AM,IB 3330,Jlemley,16,/,28,0,5.3,5.3,11,3L01,AA,
Spring 2018,North,1839,ABE 031 11,ABE MATH LEVEL 3,5,DAILY,11:00 AM,11:50 AM,IB 3309,Cancel 03/01,0,/,0,0,0,0,,,AA,
Spring 2018,North,1831,ABE 040 01,ABE/HS 21 LANG ARTS,5,DAILY,9:00 AM,9:50 AM,IB 3330,Jlemley,8,/,28,0,2.7,2.7,,,AF,
Spring 2018,North,1820,ABE 041 01,ABE MATH LEVEL 4,5,DAILY,11:00 AM,11:50 AM,IB 3409,Aabeyta,36,/,28,0,12,12,11,3L01,AA,
Spring 2018,North,1840,ABE 041 11,ABE MATH LEVEL 4,5,DAILY,11:00 AM,11:50 AM,IB 3309,Cancel 03/01,0,/,0,0,0,0,,,AA,
Spring 2018,North,1814,ABE 042 01,ABE/HS 21 SCIENCE,5,DAILY,12:00 PM,12:50 PM,IB 3330,Cancel 03/26,0,/,28,0,0,0,,,AA,
Spring 2018,North,1827,ABE 049 I2,BASIC SKILLS PHLEBOTOMY,2,T,12:00 PM,1:50 PM,CC 3350,Cancel 02/08,0,/,0,0,0,0,,,AA,


```
It's still not technically tidy per Wickham, but it served my needs at the time.  

After spending a few days writing this and some other versions of this scripts, about 2 weeks later I started over and made a different scrip, titled, FileNameCreator.py.  This is basically the same script, just cleaned up, better ogranized.d  I'm showing these two scripts as a demonstration of progress. 



# R script to tidy and visualize Salary of College Staff, Admin, and Faculty

This did a combination of webscraping from a few different sources to tidy and transform variables to analyze different employee groups in the Seattle Colleges. The most difficult problem is that there is no standard job titles for admin and staff.  Faculty generaly have the word faculty in their job title, but not 100%.  Admin is the most difficult with directors, executive directors etc.  Compicating this is that some staff were called "executive assistants", which meant that I need to filter them out from the admininstrative positions.  Executive assistants might earn 40k per year, while executive directors may earn 90k.  This used a lot of regular expressions.  




# R script to teach binomial simulations, central limit theorem, intuition about large numbers



# R script to usse object oriented programming 
