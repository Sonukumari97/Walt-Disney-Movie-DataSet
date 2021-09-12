# Walt-Disney-Movie-DataSet
To know which elements that we need to target in our python code, we need to first inspect the web page.

To gather data from wikipedia page of List of Walt Disney Pictures films we can inspect the page by right clicking on the element of interest and select inspect. This brings up the HTML code where we can see the element that each field is contained within.

Since the data is stored in a table, it will be straight forward to scrape with just a few lines of code.

All results are contained within table called in <tr> elements and these are all visible on the one page. This will not always be the case and when results span over many pages you may need to either change the number of results displayed on a webpage, or loop over all pages to gather all the information.
On the League Table webpage, a table containing 100 results is displayed. When inspecting the page it is easy to see a pattern in the html. The results are contained in rows within the table:
To create a dataset using wikipedia webpage we need following library :
 - BeautifulSoup :    used for web scraping
    - BeautifulSoup helps us to handle the html.
 - request :         request(Https) is used to either retrieve data from a specified URI or to push data to a server.
 - re(regular expression) :   used for string searching and manipulation
 - json :      to store movie dictionary 
 - pickle :    to store python object like datetime 
 - pandas :    to make a dataframe and save as a csv file 

after creating dataset we do some analysis like :
 - handling NaN value
 - visualizing using matplotlib and seabon library 
