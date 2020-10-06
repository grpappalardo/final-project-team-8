# Final Project

**Script 1**

This script extracts 5-day weather forecast information from the National Weather Service website using the BeautifulSoup library. Functionality was added to allow the user to input latitude and longitude in decimal degrees. This information is then formatted for readability (fixing spacing issues present in the scraped data), as well as converted to all uppercase.

We found that Script 1 provided an incomplete formatting solution: after fixing all the formatting issues for one set of weather conditions, more issues would appear as the weather changed. Editing individual items using  ```.replace()``` is not a very efficient way to format a constantly-changing weather forecast. However, as of 10/6/20 at 10 AM, the forecast is correctly formatted.

The user inputted latitude and longitude is converted into strings and placed into the National Weather Service URL through concatenation. The URL is used to access the weather forecast, and the relevant elements on the page are selected and scraped. The forecast is stored in a list, and then ```for day in forecast``` is used to edit the content for formatting issues that remain. In order to have ideal readability, the forecast information scraped from the National Weather Service website is edited using the ```.replace()``` method, and these edited aspects are all printed for the user.

**Script 2**

This script explores the results of an investigation undertaken within a humanitarian organization tasked with allocating funding throughout Kenya’s counties. As a result of a drop in funding, organization staff members were asked to vote (only once!) for one county whose programs were deemed “critical,” OR for whose resources were most plentiful, in order to maximize the impact of the organization’s humanitarian work. 

Challenge 1 defines a function that takes a county name as an argument and returns the number of votes for that particular county. With a county passed as the argument, the vote_count function uses a counter to add up the total number of times a county was listed as a vote in the file. This information is then printed using string concatenation.

Challenge 2 processes the KEcounty_votes.txt file with separate functions to munge a string to make it easy to match against, checks if someone has voted before, and finally counts the vote.

The munge_data function strips blank spaces at the beginning and end of the datum, makes all text lowercase, then puts it in title format. Then it removes extra blank spaces and corrects a misspelled county found in the file.

The valid_voter function determines if it is True or False that a vote is valid. The munge_data function is called to munge the voter information, then a list is created. If the name is already in the list, an alert is created and the function is returned as False. If not, the vote is counted and the function is returned as True.

The count_votes function determines, using a dictionary, how many legitimate votes were cast for each county. The KEcounty_votes.txt is munged and split so that the name and the vote are separate. If the vote is valid, per use of the valid_voter function, it is added to the counts dictionary. This information is output using concatenation. 

Challenge 1 was much more straightforward than Challenge 2. While Challenge 2's functions themselves are fairly straightforward, putting the lines of code together in a logical way was difficult, especially when they returned unexpected results (we both experienced an error where only 1 county with 1 vote was returned, ```Nairobi County: 1```.
Making the functions fit together was a new and exciting aspect of Challenge 2 compared to earlier work in the class. In order for the ```count_votes``` function work, the ```valid_voter``` function must check for fraud, and the ```munge_data``` function is used in both later functions to ensure correct reading of the file's information.
Stackoverflow.com was a very useful resource for refreshing how to write certain parts of the code, for example the method .lower(). Aaron Deibele was also very helpful during the writing and debugging process.
 Having a partner was very helpful because we had a peer resource for getting unstuck on specific tricky parts of the code. In addition, our different perspectives meant we were able to learn from one anothers’ thought process and write final scripts that were carefully considered and reviewed from multiple angles. 

