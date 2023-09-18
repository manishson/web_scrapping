# web_scrapping
Data Science Internship Assignment
ETL Pipeline

OVERVIEW
This assignment requires you to put your web scraping abilities to use! Most people are familiar with BeautifulSoup and Selenium as the top libraries for web scraping. This assignment will require you to use these technologies to scrape and clean some transactional data from a government website and set up an API to query that data. 
TO-DO
Scrape the following Mumbai Government website for Real Estate data using Selenium - 
thttps://pay2igr.igrmaharashtra.gov.in/eDisplay/propertydetails

You may use the following inputs - 
District: मुंबई उपनगर
Taluka: अंधेरी
Village: बांद्रा
Select Year: 2023
Enter Doc/Property/CTS/Survey no/Reg. Year: 2023
Click on the search button; once data is loaded, select “50” in the Record Details section to display all the data simultaneously (at once). 
Translate this data using right-click (Translate to English option, or you can install the Google Translate Extension and use it to translate the data on the page to English - Please ensure that all the data is translated by scrolling through these 50 records once).
You are required to scrape the first 50 entries of the table that comes after search results are loaded (including the index2/list no. 2 link embedded in the blue button on each row), store it in a dataframe, and subsequently store it in a Postgres Table. 
Clean the Data (Make it uniform, make sure correct/appropriate datatypes are used for each column, convert dates to a standard format, remove outliers, etc.)
Store the Data in a Postgres table with appropriate column names and data types.
When the Postgres table is set up, you must set up API Endpoint (Hint - you can use Flask) from where we can fetch the data based on Document No. or Year of Registration (not date, but year) using each endpoint. 
Notes
Will write column should be referred to by Buyer name 
Will write Down column can be referred to as the Seller Name.
It’s not necessary to automate the captcha entry part for now. You may enter it manually for now.
Bonus Points
Bonus points if you can develop an endpoint that enables us to do a partial text search. Basically, We should be able to do a partial search on the buyer's or seller's name (Second and First Party) or search for the partial address from the other Information column. 
(For example, if the Buyer's name is Mihir Yadav Agrawal, then if I search for just “Mihir” or “Yadav” using the endpoint. I should get all the transactions where that text is present as either Buyer or Seller.
Pay due importance to code quality, code documentation and schema definitions.
Bonus points if you can automate all the processes/steps involved in the process.
