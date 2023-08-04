# J124 Final Project: UC Berkeley admissions by ethnicity
## By Matthew Yoshimoto
### Data Analysis Process 
The first step of my analysis was to join the [data from UC Berkeley’s admissions from 2012 to 2022](https://www.google.com/](https://www.universityofcalifornia.edu/about-us/information-center/admissions-source-school)) onto one spreadsheet. I next inserted a column of the admissions year to the left of each school name. To clean my data, I had to unmerge the combined cells and then use the [array formula](https://infoinspired.com/google-docs/spreadsheet/fill-merged-cells-in-google-sheets/) to fill the merged cells down. This made it so that the schools and cities were now listed in every row. At this point, I could begin my data analysis. This is the [data set I analyzed in Google Sheets](https://docs.google.com/spreadsheets/d/1oYrYav8eZLnbJ14ZFdc4DFqpaceefVChhTK2Kuado08/edit#gid=0).  <br/>
!['Data Analysis Process', 'Data Analysis Process'](/1.jpg) <br/>

### Scope of Analysis
1.  Which county had the overall highest number of Hispanic/ Latinx admits from 2012 to 2022? <br/>
2.  What was the percentage change of Asian admits from 2012 to 2022? <br/>
3.  From 2012 to 2022, what were the top ethnicities of students who were admitted most often? How does this compare to the top ethnicities of students who applied most often? <br/>
4.  From 2012 to 2022, which counties had the highest number of white enrollees? How many counties had zero white enrollees?  <br/>
5.  From 2012 to 2022, what was the average number of international applicants per each county? Only include the counties that had an average of seven or more international applicants. Round to the nearest hundredths place.  <br/>
6.  Which school had the highest number of total applicants, and in which year did this occur? What was the average number of total applicants across all schools from 2012 to 2022? Round to the nearest hundredths place.  <br/>
7.  In 2018, what were the top counties with the highest number of total African American applicants, admits, and enrollees? <br/>

### Key Assumptions
*  The schools listed are all public high schools in California, including charter schools. <br/>
*  The abbreviation “App” represents applicants, or students who make a formal application to attend the University of California. <br/>
*  The abbreviation “Adm” represents admits, or students who have been made a formal offer of admission to attend the University of California. <br/>
*  The abbreviation “Enr” represents enrollees, or students who have accepted an offer of admission and are enrolled at the University of California. <br/>

### Analysis 1: Which county had the overall highest number of Hispanic/ Latinx admits from 2012 to 2022? 
1.  Create a pivot table with “Count” as the first row, followed by “County/State/Territory” as the next row. Set “Hispanic/Latinx” as the column. Summarize by “SUM.” 
!['Analysis 1', 'Analysis 1'](/2.jpg)<br/>
2.	Make sure to look at the admits category. Feel free to minize the applicants and enrolled categories.
!['Analysis 1', 'Analysis 1'](/3.jpg)
3.	Copy and paste without formatting the admits values to a new sheet.!['Analysis 1', 'Analysis 1'](/4.jpg)
4.	Sort the column “Hispanic/Latinx” from Z → A to find the county with the highest number of Hispanic/Latinx admits.

#### *  As shown, Los Angeles County has the highest number of Hispanic/Latinx admits at UC Berkeley from 2012 to 2022, with a total of 3041 students. 


### Analysis 2: What was the percentage change of Asian admits from 2012 to 2022?

1.  Create a pivot table with “Count” as the first row, followed by “Year” as the next row. Set “Asian” as the column. Summarize by “SUM.” 
!['Analysis 2', 'Analysis 2'](/5.jpg)
2.  Make sure to look at the admitted category. Feel free to minize the applied and enrolled categories. 
!['Analysis 2', 'Analysis 2'](/6.jpg)
3.  Copy and paste without formatting the admitted values to a new sheet. 
!['Analysis 2', 'Analysis 2'](/7.jpg)
4.  Use the formula (NEW-OLD)/OLD or (B12-B2)/B2 to calculate the percentage change  of Asian admits from 2012 to 2022. *Make sure to change the formatting of the percentage change to a percentage. 
!['Analysis 2', 'Analysis 2'](/8.jpg)
#### *  As shown, the number of of Asian admits from 2012 to 2022 increased by 30.75%. 


### Analysis 3: From 2012 to 2022, what were the top ethnicities of students who were admitted most often? How does this compare to the top ethnicities of students who applied most often?

1.  Create a pivot table with “Count” as the first row, followed by “Year” as the next row. Set all ethnicities (“African American,” “American Indian,” “Hispanic/ Latinx,” “Pacific Islander,” “Asian,” “White,” “Domestic Unknown,” “Int'l”) as the column. Summarize all by “SUM.” !['Analysis 3', 'Analysis 3'](/9.jpg)
2.	Make sure to look at the admitted category. Feel free to minize the applied and enrolled categories. 
!['Analysis 3', 'Analysis 3'](/10.jpg)
#### *	As shown in the admits total row, Asian students were admitted the most often (at 30,671 students), followed by white admits (at 13,226 students) and Hispanic/Latinx admits (at 7,979 students). 

3.  Looking at the same pivot table, expand the applied category and minimize the admitted category. 
!['Analysis 3', 'Analysis 3'](/11.jpg)
#### *  As shown in the applicants total row, Asian students applied the most often (at 215,551 students), followed by Hispanic/Latinx applicants (at 111,788 students) and white applicants (at 106,278 students). 


### Analysis 4: From 2012 to 2022, which counties had the highest number of white enrollees? How many counties had zero white enrollees? 

1.  Create a pivot table with “Count” as the first row, followed by “County/State/Territory” as the next row. Set “White” as the column. Summarize all by “SUM.” 
!['Analysis 4', 'Analysis 4'](/12.jpg)
2.	Make sure to look at the enrolled category. Feel free to minize the applied and admitted categories. 
!['Analysis 4', 'Analysis 4'](/13.jpg)
3.  Copy and paste without formatting the enrolled values to a new sheet. 
!['Analysis 4', 'Analysis 4'](/14.jpg)
4.	Sort the column “SUM of White” from Z → A to find the county with the highest number of white enrollees.
!['Analysis 4', 'Analysis 4'](/15.jpg)
#### *  As shown, Los Angeles County has the highest number of white enrollees from 2012 to 2022, with a total of 1249 students. This is followed by San Diego County (at 624 enrollees) and Orange County (at 575 enrollees). 

5.  Now create another pivot table using the data on this new sheet. 
!['Analysis 4', 'Analysis 4'](/16.jpg)
6.  Set “White” as the row and set “County/State/Territory” as the column. Summarize by “COUNTA.” 
!['Analysis 4', 'Analysis 4'](/17.jpg)
#### *  As shown, there are 23 counties that never had a white enrollee from 2012 to 2022. 


### Analysis 5: From 2012 to 2022, what was the average number of international applicants per each county? Only include the counties that had an average of seven or more international applicants. Round to the nearest hundredths place. 

1.  Create a pivot table with “Count” as the first row, followed by “County/State/Territory” as the next row. Set “Int’l” as the column. Summarize by “AVERAGE.” !['Analysis 5', 'Analysis 5'](/18.jpg)
2.  Make sure to look at the applied category. Feel free to minize the admitted and enrolled categories. *The “DIV/0!” will appear for counties that had no international applicants. 
!['Analysis 5', 'Analysis 5'](/19.jpg)
3.  To hide all rows with “DIV/0!”, add a filter for “Int’l”. Uncheck the “(Blanks)” optiom. 
!['Analysis 5', 'Analysis 5'](/20.jpg) !['Analysis 5', 'Analysis 5'](/21.jpg) 

4.  To round to nearest hundredths, format the values as “Number”.!['Analysis 5', 'Analysis 5'](/22.jpg)
5.  Copy and paste without formatting the enrolled values to a new sheet. !['Analysis 5', 'Analysis 5'](/23.jpg)
6.  Sort the column “AVERAGE of Int’l” from Z → A to find the counties that had the highest averages of international applicants. !['Analysis 5', 'Analysis 5'](/24.jpg)

#### *  As shown, from 2012 to 2022, San Joaquin County had 9.67 applicants, Santa Clara County had 9.38 applicants, Alameda County had an average of 8.20 international applicants, San Diego County had 7.27 applicants, and Contra Costa County had 7.13 applicants.


### Analysis 6: Which school had the highest number of total applicants, and In which year did this occur? What was the average number of total applicants across all schools from 2012 to 2022? Round to the nearest hundredths place. 

1.  Make a copy of the original sheet of data. Sort the “All” column from Z → A to find the schools that had the highest number of total applicants. !['Analysis 6', 'Analysis 6'](/25.jpg)
#### *  As shown, Dougherty Valley High School had the highest number of total applicants (at 547 students). This occurred in 2022. 
2.  To find the average number of total applicants across all schools from 2012 to 2022, click on the “All” column and locate the “Sum” button on the bottom right of the sheet. !['Analysis 6', 'Analysis 6'](/26.jpg)
3.  Click on the “Sum” button and select “Avg”. !['Analysis 6', 'Analysis 6'](/27.jpg)

#### *  As shown, the average number of total applicants across all schools from 2012 to 2022 was 25.73 applicants. 


### Analysis 7: In 2018, what were the top counties with the highest number of total African American applicants, admits, and enrollees?

1.  Create a pivot table with “Year” as the first row, followed by “County/State/Territory” as the next row. Set “African American” as the column. Summarize by “SUM.” !['Analysis 7', 'Analysis 7'](/28.jpg)
2.  Make sure to look at 2018 category. Feel free to minize the 2012, 2013, 2014, 2015, 2016, 2017, 2019, 2020, 2021, and 2022 categories. !['Analysis 7', 'Analysis 7'](/29.jpg)
3.  Copy and paste without formatting the values from 2018 to a new sheet. !['Analysis 7', 'Analysis 7'](/30.jpg)

4.  Sort the column “SUM of African American” from Z → A to find the county with the highest number of total African American applicants, admits, and enrollees.
!['Analysis 7', 'Analysis 7'](/31.jpg)
#### *  As shown, Los Angeles County had the highest number of total African American applicants, admits, and enrollees. This is followed by Alameda County (at 205 students) and San Diego County (at 125 students). 
