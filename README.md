# Deliverable Three: Election Analysis Challenge 

## Overview of Election Audit
The goal of the analysis of the election audit was to analyze the results of the 2019 election.  We were looking to breakdown the ballots by both the county they were cast in, as well as by who they were cast for.  In order to do this, we created a script in python that was able to calculate the total amount of votes, where they were cast, and who they were cast for.  That analysis made us able to determine how mnay votes each candidate received, and from which county those votes came from.

## Election-Audit Results

- There were a total of 369,711 votes cast in the congressional election.

- Of those 369,711 votes, 306,055 (82.8%) were cast in Denver county, 38,855 (10.5%) were cast in Jefferson county, and 24,801 (6.7%) were cast in Arapahoe county.

![Alt_Text](https://github.com/Nickguild1993/Election_Analysis/blob/master/Vote%20by%20county%20Bar.png)

- Denver county, with 306,055 votes, had by far the largest voting bloc of the three counties, making up 82.8% percent of the total amount of votes.

- Diana DeGette received the most votes with 272,892 (73.8% of the total), Charles Casper Stockham received the second most with 85,213 votes (23% of the total), and lastly, Raymon -Anthony Doane received 11,606 votes (3.1% of the total votes cast).

![Alt_Text](https://github.com/Nickguild1993/Election_Analysis/blob/master/Total%20vote%20pie%20chart.png)

- Diana DeGette won the election with 272,892 out of 369,711 possible votes.  Her percentage of the total vote was 73.8%.

## Election-Audit Summary
What the team was able to accomplish in this audit- breaking down the total vote count by county and by candidate, is not limited to this election.  What we did can be modified by changing the values (like the counties and candidates) of the variables so that a similar audit could be run for a different election.  As long as we have the raw data that gives us each voters **ballot ID, county**, and **candidate**, this analysis can be readily applied to a new dataset.  

For example, if you had an election that took place in Travis, Hays, and Williamson counties instead of the three from this audit, all we would have to change is the **list variable** that tracks counties. By changing the **counties = [ ]** to match the CSV (comma seperated values) file, we can pull the unique names of the counties by using the script **county_name = row[x]** where the **x** represents which column index (n-1) the **county** value appears in.  

Additionally, if we had another election with it's own candidate's we can again very easily modify this script to run an analysis of those candidates and how many votes they received.  By changing the values in **candidate_name** variable to match those in the new election, we can again breakdown how those candidates performed relative to each other and ultimately, who won the election.  By pulling their names from the CSV file, the script **candidate_name = row[x]** where like in the above example, **x** represents the column index that the **candidate name** appears in.  

In essence, what we have created isn't just an election audit of the 2019 congressional race, but a highly customizable script that can have values readily plugged into it to run analysis of any election that the election commission is overseeing.  This script has the power to drastically reduce the amount of time that an audit takes by automating the entire process- from reading the CSV file to writting a text file with the results.  
