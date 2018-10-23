# Web-Scraping-and-Document-Database
<B>Objective</B><P>
Build a web application that scrapes various websites for data related to the Mission to Mars and displays the information in a single HTML page following outlines below.<p>
    <b>Step 1 - Scraping</b><p>
Complete initial scraping using Jupyter Notebook, BeautifulSoup, Pandas, and Requests/Splinter.<p>
1.	Scrape the NASA Mars News Site(https://mars.nasa.gov/news/) and collect the latest News Title and Paragraph Text. Assign the text to variables.
2.	JPL featured space image
o	JPL featured space image website https://www.jpl.nasa.gov/spaceimages/?search=&category=Mars
o	Use splinter to navigate the site and find the image url for the current featured Mars image and assign the url string to a variable called `featured_image_url`. 
o	 Save a complete url string for this image.
3.	Mars Weather
o	Mars weather twitter account https://twitter.com/marswxreport?lang=en
o	 Scrap the latest Mars weather tweet from the page. Save the tweet text for the weather report as a variable called `mars_weather`.
4.	 Mars Facts
o	Visit the Mars Facts webpage [here](http://space-facts.com/mars/) and use Pandas to scrape the table containing facts about the planet including Diameter, Mass, etc.
o	Use Pandas to convert the data to a HTML table string.
5.	 Mars Hemispheres
o	Visit the USGS Astrogeology site (https://astrogeology.usgs.gov/search/results?q=hemisphere+enhanced&k1=target&v1=Mars) to obtain high resolution images for each of Mar's hemispheres.
o	Save both the image url string for the full resolution hemisphere image, and the Hemisphere title containing the hemisphere name. Use a Python dictionary to store the data using the keys `img_url` and `title`. 
o	 Append the dictionary with the image url string and the hemisphere title to a list. This list will contain one dictionary for each hemisphere.
<p><b>Step 2 - MongoDB and Flask Application</b></p>
<p>Use MongoDB with Flask templating to create a new HTML page that displays all of the information that was scraped from the URLs above.

