# Final Project

**Script 1**

This script extracts 5-day weather forecast information from the National Weather Service website using the BeautifulSoup library. Functionality was added to allow the user to input latitude and longitude in decimal degrees. This information is then formatted for readability (fixing spacing issues present in the scraped data), as well as converted to all uppercase.

We found that Script 1 provided an incomplete formatting solution: after fixing all the formatting issues for one set of weather conditions, more issues would appear as the weather changed. Editing individual items using  ```.replace()``` is not a very efficient way to format a constantly-changing weather forecast. However, as of 10/6/20 at 10 AM, the forecast is correctly formatted.

**Script 2**

These scripts explore the results of an investigation undertaken within a humanitarian organization tasked with allocating funding throughout Kenya’s counties. As a result of a drop in funding, organization staff members were asked to vote (only once!) for one county whose programs were deemed “critical,” OR for whose resources were most plentiful, in order to maximize the impact of the organization’s humanitarian work. 

The first script (Challenge 1) defines a function that takes a county name as an argument, and returns the number of votes for that particular county.

The second script (Challenge 2) processes the KEcounty_votes.txt file with separate functions to munge a string to make it easy to match against, check if someone has voted before, and finally to count a vote.

Challenge 1 was much more straightforward than Challenge 2. While Challenge 2's functions themselves are fairly straightforward, putting the lines of code together in a logical way was difficult, especially when they returned unexpected results (we both experienced an error where only 1 county with 1 vote was returned, ```Nairobi County: 1```.
Making the functions fit together was a new and exciting aspect of Challenge 2 compared to earlier work in the class. In order for the ```count_votes``` function work, the ```valid_voter``` function must check for fraud, and the ```munge_data``` function is used in both later functions to ensure correct reading of the file's information.
