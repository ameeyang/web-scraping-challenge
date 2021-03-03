# web-scraping-challenge
mission_to_mars
In this assignment,a web application is designed to scrapes various websites for data related to the Mission to Mars and displays the information in a single HTML page. The following outlines what you need to do.

Step 1 - Scraping
Initial scraping is done using Jupyter Notebook, BeautifulSoup, Pandas, and Requests/Splinter.

Jupyter Notebook file called mission_to_mars.ipynb is created to complete all of your scraping and analysis tasks. The following outlines what you need to scrape.
NASA Mars News
The NASA Mars News Site is scraped collect the latest News Title and Paragraph Text.
Example:
news_title = "NASA's Next Mars Mission to Investigate Interior of Red Planet"

news_p = "Preparation of NASA's next spacecraft to Mars, InSight, has ramped up this summer, on course for launch next May from Vandenberg Air Force Base in central California -- the first interplanetary launch in history from America's West Coast."


### JPL Mars Space Images - Featured Image

* Visit the url for JPL Featured Space Image [here](https://www.jpl.nasa.gov/spaceimages/?search=&category=Mars).

* Using splinter to navigate the site and find the image url for the current Featured Mars Image and assign the url string to a variable called `featured_image_url`.

* Making sure to find the image url to the full size `.jpg` image.

* Making sure to save a complete url string for this image.

```python
# Example:
featured_image_url = 'https://www.jpl.nasa.gov/spaceimages/images/largesize/PIA16225_hires.jpg'
Mars Weather
Visiting the Mars Weather twitter account here and scraping the latest Mars weather tweet from the page. Saving the tweet text for the weather report as a variable called mars_weather.
# Example:
mars_weather = 'Sol 1801 (Aug 30, 2017), Sunny, high -21C/-5F, low -80C/-112F, pressure at 8.82 hPa, daylight 06:09-17:55'
Mars Facts
Visiting the Mars Facts webpage here and using Pandas to scrape the table containing facts about the planet including Diameter, Mass, etc.
Mars Hemispheres
Visiting the USGS Astrogeology site here to obtain high resolution images for each of Mar's hemispheres.

The dictionary is appended with the image url string and the hemisphere title to a list. This list will contain one dictionary for each hemisphere.

# Example:
hemisphere_image_urls = [
    {"title": "Valles Marineris Hemisphere", "img_url": "..."},
    {"title": "Cerberus Hemisphere", "img_url": "..."},
    {"title": "Schiaparelli Hemisphere", "img_url": "..."},
    {"title": "Syrtis Major Hemisphere", "img_url": "..."},
