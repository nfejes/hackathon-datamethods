# Hackathon 10/6 - Data Methods and Design

# Team Members

* [name-of-a-team-member](URL to this member's github account)
* [name-of-a-team-member](URL to this member's github account)
* [name-of-a-team-member](URL to this member's github account)
* [name-of-a-team-member](URL to this member's github account)
* [name-of-a-team-member](URL to this member's github account)

# Part 1: Data Science Fundamentals


## Q1: There are generally 2 situations you'll start from when approaching a question of data: a) You designed and collected the data yourself OR b) You have to work with a data set you've been given access to.  What do you think makes these 2 starting points different?  How might it change what analysis you'll do?

If you collect the data yourself you most likely have a goal with the data collection, and design the database and fields in a way so that you can use it for a specific purpose. If someome else has collected the data they might have had different reasons for collecting the data, such as only to be able to inspect specific events and not the whole data set.

(For the following set of questions we'll assume we're in situation A - you are going to design your own data collection)

## Q2: What factors go into deciding what data format to use?  Under what circumstances may you use different data types? (i.e., JSON, CSV, Key-Value Store, txt documents)
**JSON:** If you want to store unstructured data, like data pulled from website where you might not know exactly what data you will get. If the data is nested in some way.

**CSV:** If you know exactly what data fields you will get, and the possible values are limited in size.

**Key-Value Store:** 

**txt documents:** Store text.

## Q3: Once you've chosen a format, you'll need to determine fields to capture and store.  A common approach for this involves determining what QUESTIONS you want to ask of your dataset.  For the following examples, please respond with which field(s) your may need to answer the questions needed:
1. You're working for a company that tracks data on public transportation, you know you'll want to be able to ask "What percentage of a time is a bus/train late?"
2. You're working for a school district, and you need to be able to help the principal answer the question "Which teachers are most successful at getting students interested in extra-curricular educational activities (e.g., Math Team, Quiz Bowl, Science Olypiad, Robot Building, etc)? 
3. You're starting a social networking website that helps friends choose what to do on a Friday night, and you need to be able to answer the question, "Who made the suggestion that led to the final decision?"

### Answers:
1. Time of arrival/leave from station, time supposed to arrive/leave, time difference
2. Name/ID of students mapped to classes and extra-curricular activities, Name/ID of teachers mapped to classes
3. All events, with users and references to previous related events

## Q4: Now you need to decide how you'll query your data.  What are the costs and benefits of the following options: 
1. Store the data raw and load it into a Python or JavaScript Shell for analysis.  
2. Periodically dump the data into a database (like Mongo) and query it.
3. Build a webserver and write an API that dumps and queries that data in your database.

### Answers:
1. You can't work with large data sets / You have quick and easy access to your data
2. Slower access time / You can work with large data sets, do analysis on bigger data
3. Slow access time / Store lot of data


## Q5: You've now set up your database and have a website with 10,000 users, but have realized that you forgot a much needed field (say, an ID number for each user).  What do you do and how might different database designs have helped this situation?

Rebuild the database. Add fields if you can.

---------------

(For this section, you may need to do some online research to answer the questions.)

## Q6: What is a Baysian Classifier?  What is it used for?
[Response]

## Q7: What is a simple graph you could generate to check for outliers in a dataset?
[Response]

## Q8: What is a Null Hypothesis?
The null hypothesis refers to a general statement or default position that there is no relationship between two measured phenomena.

----------

Answer the following questions using this scenario: You just got a HUGE dataset from Spotify where each entry contains these fields -> [username, song, # of times played, user rating, genre]

## Q9: How would you figure out the most popular song?
group data by song and calculate sum(# times played) and avg(user rating)

## Q10: How do you determine what genre a certain user likes the most?
for that user, group the data by genre and calculate sum(# times played) and avg(user rating)

Both the # times played and user rating should be indicators of the genre the user likes the most

## Q11: How do we match 2 users that we think may want to share playlists?
Generate "fingerprints" based on how much a certain user likes a specific genre and match people with similar fingerprints.

## Q12: What assumptions would you have before digging into Spotify data?  How would you test them?
People in general listen more to the music they like. Test by looking at correlation between user rating and # times played.

----------

Answer these last questions generally.

## Q12: What is a correlation and how do you find them in a data set?
[Response]

## Q13: How can correlations help us tell a story with our data? 
[Response]

## Q14: Let's think about data science as a way to tell a story about some data.  Why would I want to bring a second data set into my story?
[Response]

## Q15: This one's just for fun.  How percent of the time do you expect to actually get the result you wanted?
[Response]


# Part 2: Analyzing Your Data

While there are many tools to do this analysis, we will use the JS library Gauss to accomplish this task since everyone should have used it by now.

## Screenshot of Data in Gauss
![screenshot of data in gauss](image.png?raw=true) 

## Most Frequent Value
[cut and paste command used and the output it produced]

## Range of data
[cut and paste command used and the output it produced]

## Biggest Change
[cut and paste command used and the related snippet from the output]

## Shape of data
[Describe]

## Threshold
[Value]

## Percentage above/below
[Command and output]

## Yes/No + Justification
[Answer and any images/snippets to justify]

# Part 3: Project Design Exercise

## Link to the device or devices you're interested in using
* [device1](URL to this device)
* [device2](URL to this device)

## What it would measure and how?
[Response]

## Where you'd put it in the lobby?
[Location]

## What problems could threaten the validity of your data?
[Response]

## How often to sample and when to make a data dump?
[Response]

## Resulting viz.
[Describe or link to example]

## Timing trigger
[Necessary? Why? and How?]

