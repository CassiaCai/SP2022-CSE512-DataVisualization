### Notes
- Created using the Vega-Lite API in Observable (JavaScript)
- Data set: monthly hours of sunshine in major U.S. cities

For more information about the dataset, including download links for CSV and JSON formats, see https://observablehq.com/@uwdata/hours-of-sunshine.

![a1_image](https://user-images.githubusercontent.com/52092892/162023770-e27c34f8-cd8a-44b8-a181-73a1f0b68e2a.png)

### Write-up
Sunshine duration is used as a measure of cloudiness of a location rather than solar insolation, which depends on latitude and how Earth orbits the sun. The question I chose to ask is about the relationship between latitude and the monthly variability of sunshine duration, or cloudiness. Question: What is the relationship between latitude and monthly variability of sunshine duration?

From my image, we observe that in May, June, July, and August, the monthly variability of sunshine duration is smaller at lower latitudes. In the other months, generalizing is more difficult. We also observe that the seasonal cycle is weakest in Miami followed by New York. Both cities are in the East category. 

Given a small data set consisting of monthly hours of sunshine in 6 major U.S. cities, I noticed that the locations of the 6 cities could roughly be separated into three categories (based on longitude), West, middle, and East, with 2 cities in each category. Because I was only interested in monthly variability, I removed the average number of sunshine hours from each timeseries. I then generated three separate bar graphs (one for each category). The choice to use bar graphs is driven by the ease of comparison between the two cities in each category. The difference can be easily approximated by eye. This is further facilitated by the color choice of the bars. For cities at higher latitudes, I used solid orange bars. For cities at lower latitudes, I used unfilled bars with a black edge. I chose to use orange and black because orange can be used to indicate sunshine (association with sunlight). The choice to use black simplified the design so that there is minimal visual clutter. The y-axis scale for the bar graphs ranges from -150 to 150 hours. This allows 0 hours to be right in the middle. This makes looking at and understanding variability easier. 

I found it more meaningful to retain the monthly number of hours rather than calculate an average daily number of hours for each month because I am interested in understanding the strength of the seasonal cycle. I also included on the top right a small map of the U.S. with the 6 cities as points. This map is small because it is not the main message of my image. However, including it allows the audience to see the locations of these 6 cities. Some caveats are that the longitudes of the cities in each category are not the same. If they were, then the comparison would be more direct. Another useful addition would be a map of the average climate of the U.S. A deeper understanding of what affects cloudiness might result in a different categorization scheme. 
