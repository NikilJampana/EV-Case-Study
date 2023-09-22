# EV-Case-Study
Teslas have been popping up everywhere around me, so I decided to take a deeper dive into understanding their recent surge in popularity in the form of a case study. 

# 1. Objective
EV owners and prospective owners have had growing concerns about EV charging according to a recent J.D. Power report. A company is trying to decide what locations are best to place EV charging stations in Washington. The task is to use existing data on EV populations and charging station availabity to identify cities to prioritize for placement of charging stations. The main data sets being used are an Electric Vehicle Population Dataset for the state of Washington and Federal records on Alternative Fueling Stations.

# 2. Data Cleaning and Preparation Steps
While there was little work to be done on the Electric Vehicle Population Dataset for the state of Washington, I did have to clean the Alternative Fueling Stations document. While it was originaly designed to represent several different types of alternative fuel across the United States, I filtered and adjusted the document to only look for electric charging station in Washington. In addition, the date format provided on the document wasn't compatible with Google Sheets, so I ran the csv through SQL to transfer it to a useable format for me. My data all originated from public data repositories from the U.S. Government, which verified its credibility for me and ensured that no licensing would prevent its personal use. I prefered to use Excel when analyyzing the data at hand because of its ease of use and how well-formatted the pre-existing data was. For my purposes, there was no major cleaning that needed to be done.

When considering ROCCC, our data is:
- Reliable, because the sample size is the whole population.
- Not original, because it was pulled from a third party website.
- Not wholly comprehensive because it doesn't contain a wide variety of data useful to our project.
- Somewhat current, since our data sets span from 2019 to 2021.
- Well cited, because it documents it capture and methodology

# 3. Analysis Steps
To start, I approached this analysis trying to analyze two major factors that might impact the average EV user regarding charging stations. These were the distance to the average EV charging station and how crowded EV stations might be. To analyze these best using the data I had, I created and graphed two seperate metrics designated by city. 

### 1. Chargers per Electric Vehicle
This metric was intended to gauge how crowded EV chargers might be in the city, with a higher number indicating less crowding. For the top 20 EV owning cities in the state, the results looked like this:

![alt text](https://github.com/NikilJampana/EV-Case-Study/blob/main/Graphs/Chargers%20per%20EV.png?raw=true)

### 2. Stations by City Size. 
This metric was intended to show the average distance an EV owner might have to drive to get to a charging station, with a higher number again indicating a farther distance. For the top 20 cities, the results looked like this:

![alt text](https://github.com/NikilJampana/EV-Case-Study/blob/main/Graphs/Stations%20By%20City%20Size%20(1).png?raw=true)

These results gave me a general indication of what cities seemed most in the need of more stations. To combine these two metrics, I multiplied the Chargers per EV values by 75 to scale it to the stations by city size values and combined them into a single chart:

# 4. Results
The stacked bar graph resulting from my analysis looks as follows:

![alt text](https://github.com/NikilJampana/EV-Case-Study/blob/main/Graphs/TotalChart.png?raw=true)

When looking at our results graph, a few major results become clear. 

- None of the 5 largest EV owning cities rank low on this list, indicating that cities with the largest EV owning populations have already focused on providing chargers.
- The 5 lowest scoring cities are: Sammamish, Kent, Bothell, Mercer Island, and Tukwila. These would be the areas I suggest to the company to prioritize.
- In particular, Sammamish has very low ratios for both metrics, and should therefore be heavily prioritized.


# 5. Future Action
While my analysis was able to suggest several cities to prioritize that would likely be well met with increased charging stations, there are many more areas that could be covered that I simply didn't have the data to analyze. One of the most prominent of these is the price points of various EVs and how that affects EV owner satisfaction. Further more, my assumption that both EV charger distance and overcrowding hold equal weight in the eyes of the consumer may not be completely accurate, so surveys might help bridge that gap in understanding and let the company know how these factors inter-relate. In addition, with more precise data on the location of various charging stations, you can accurately pinpoint the maximum, minimum, and average distance a EV owner would take to reach a charger. I would suggest utilizing customer satisfaction surveys and gathering more consumer data as a next step to this process on identifying key areas, but I believe this initial analysis would guide a company in the right direction for optimally placing EV chargers.
