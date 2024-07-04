# TN-Library-Process
 The data, notebooks, and process notes for TN-Library-Project
---
## Content Description
I called this project "Reading Between the Lines: How are kids interacting with Tennessee public libraries?" I had initially aimed to accomplish painting a picture of the average (read: median) library in Tennessee, but I found that pinpointing just one "typical" library made for boring visualizations. Between that and learning about the fact that over half of the libraries that provided data did not have a paid children's librarian, I then aimed to focus on how children interact with libraries and how libraries, in turn, interact with them.

I found that kids make up one fifth of all registered borrowers in the state and kids' content makes up about a fifth of all circulated material in the state. I found that over half of all responding libraries did not have a paid children's librarian, which led me to find that Tennessee also only has half the average number of total librarians per library when compared to the U.S. as a whole.

I also found that the average library hosted seven Summer Reading Program events, which while not explicitly children's only events are heavily marketed as ensuring summer literacy retention. That typical library hosted those events with a budget of less than $1,000, meaning that each event got just under $130 put toward its completion. Almost 85% of state libraries utilized Summer Reading Program marketing materials from a national program.

## Finding and analyzing the data

First, I found the [IMLS](https://www.imls.gov/sites/default/files/2024-06/2022_pls_data_file_documentation.pdf) documentation, which contained a breakdown of the survey sent out to libraries across the country. I was actually originally wanting to look at national data, but when I opened the raw csv file for it, I noped out.
Plus, I like Tennessee.
Anyway, then I spent a lot of time crawling around the [Tennessee Public Library Statistics](https://sos.tn.gov/tsla/services/tennessee-public-library-statistics) webpage. I thought their calculator was neat and I liked the idea of the [Tennessee Libraries By the Numbers](https://sos.tn.gov/tsla/services/tennessee-public-library-statistics) plugin that spat out categorical summaries for a library of your choice. I used those spitouts as inspiration for things to look for in the most-recent complete state [data](https://tn.countingopinions.com/pireports/report.php?f6640fe2051cf5e24d4e284f3c27c537&live).

I did initially try to download the state data as an Excel file, but when I tried to do pandas with it, it did not work because it was an html file in disguise! I had to convert the data into the friendlier csv you see here before I could dig into the numbers.

Because I was initially just painting a picture of the typical Tennessee library, my analysis looked like a lot of cleaning and some basic pandas functions. Then, I worked with a lot of .median() functions to make way for outliers. At one point, I was going to try to graph something in matplotlib, but with approximately 200 libraries, it looked like hot garbage.

At one point, I realized that several columns had *eerily similar* names. I got confused.

I got so confused that I actually called my local library and got the email address for one of the librarians that supplied the data for my branch. She was **the best.** She sent me the complete data for my local branch, which also had some extra column identifiers that were absent in both the national documentation and the state documentation. It's not in this repository because it had her personal identifying information on it, nor did I ask her permission to upload the raw data (or name her here). 

## Wins & Losses
I learned *oh-so* much about html and css doing this! Even the things that did not work, like when I tried to make an Illustrator graphic representing the average library and Summer Reading Program events, still taught me things. The more I search on StackOverflow, the more I understand what I read and the less afraid I have become about all of this.

...But I know in my soul that these visualizations are boring. Pie chart? Bar chart? Please. I wanted to have something fun and Gurman-esque, but I felt like I was missing key elements of the data for which those would have worked best. I also realized a bit too late that trying to zoom in on one "average" library doesn't leave a lot of room for fun visuals. If I had more time, I think I also would have found a way to bring in other data, perhaps from different years, to see if Tennessee has always lacked children's and young adult librarians. It's no excuse, but I am working during the program, and I was positively screenmaxxing trying to get these to work. If
