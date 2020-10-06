# Final Project

## Details about the write up:
Your write up should clearly and succinctly describe __both__ scripts. Your submitted repo need only include one `README` (that contains the write-up) and two script files. [See this example for how to structure your repo.](https://github.com/IDCE-MSGIS/sample-lab/tree/master)

**Script 1:** Briefly explain the purpose of the script, how well it functioned (or if it didn’t), and whether or not you might use something like this in the future.

**Script 2:** clearly explain what you are trying to do: even though there will be prompts in the tutorial, you should reframe these in your own words. While your comment code will help someone reviewing the code understand what it does, youre write-up should expand on these an offer more detail. Additionally, you should describe the process of writing the script: was it easy, hard, what challenges or errors did you face and how did you resolve them? If you use any resources to help write your code (e.g. Stackoverflow.com; the text book; etc.), please link to them in the body of your text. E.g. “After repeated syntax errors, I checked [Stackoverflow.com](https://stackoverflow.com/help/referencing) to find that…”  Use Markdown to format your text and link to a specific online resources that you used.

Remember: when this project is complete, we can transfer ownership of this repo to you so it will appear in your Github account and be something you can use to demonstrate your technical ability coming out of this class: so make this count! You can also use [Github's "Issues" functionality](https://guides.github.com/features/issues/) to communicate directly with your partner via Github (you can also tag Shashank and I for questions!). 

**Script 1**

This script extracts 5-day weather forecast information from the National Weather Service website using the BeautifulSoup library. Functionality was added to allow the user to input latitude and longitude in decimal degrees. This information is then formatted for readability (fixing spacing issues present in the scraped data), as well as converted to all uppercase.

We found that Script 1 provided an incomplete formatting solution: after fixing all the formatting issues for one set of weather conditions, more issues would appear as the weather changed. Editing individual items using  ```.replace()``` is not a very efficient way to format a constantly-changing weather forecast. However, as of 10/6/20 at 10 AM, the forecast is correctly formatted.

**Script 2**

These scripts explore the results of an investigation undertaken within a humanitarian organization tasked with allocating funding throughout Kenya’s counties. As a result of a drop in funding, organization staff members were asked to vote (only once!) for one county whose programs were deemed “critical,” OR for whose resources were most plentiful, in order to maximize the impact of the organization’s humanitarian work. 

The first script (Challenge 1) defines a function that takes a county name as an argument, and returns the number of votes for that particular county.

The second script (Challenge 2) processes the KEcounty_votes.txt file with separate functions to munge a string to make it easy to match against, check if someone has voted before, and finally to count a vote.

Challenge 1 was much more straightforward than Challenge 2. While Challenge 2's functions themselves are fairly straightforward, putting the lines of code together in a logical way was difficult, especially when they returned unexpected results (we both experienced an error where only 1 county with 1 vote was returned, ```Nairobi County: 1```.
