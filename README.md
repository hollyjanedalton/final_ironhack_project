## Are North Americans Really Starbucks' #1 Fans?
![](https://github.com/hollyjanedalton/final_ironhack_project/blob/main/starbucks_map.png)

[Click for 9-minute recording of live presentation](https://ironhack.zoom.us/rec/play/z_KuzP88l79dzVBAtHaR-vPE4Xi4xUGUU-C3D948G81Z7jHR7GCBa8oip2yDNDrNwbnBrP9AWwVZ6sM9.WElypAcnuo2-6udI?startTime=1660305720000&_x_zm_rtaid=v-1r2qOaSt-VQG_GldUWIA.1660487182977.ee234b4949979eb90f4b2d2092f0085f&_x_zm_rhtaid=21)

[Click for presentation slides](https://slides.com/hollydalton/deck-5b0977/fullscreen)

[Click for Kaggle dataset](https://www.kaggle.com/datasets/kukuroo3/starbucks-locations-worldwide-2021-version)

---

### Background:
I couldn't help but notice when I lived in Australia, South Africa, and Spain, that although people drink coffee everyday like many people in the US do, Starbucks coffeehouses were sparse, and just plain unpopular with locals. 

When my mom visited, one of her only requests was that wherever we stayed, there needed to be a Starbucks nearby (a true Starbucks fanatic). It was no easy feat finding an Airbnb/Hotel within walking distance to a Starbucks everytime, so, I had to wonder-- 
#### Are Americans really Starbucks #1 Fans? Where else in the world is Starbucks as popular as it is in the US?

---

### Questions:
Using Starbucks location data with webscraped global population data, I answer these questions: 

1. What countries have the most Starbucks cafes (by count), per capita, and by area (density)?
3. Where in the world does Starbucks open the earliest, and at what time?
4. Where are the two Starbucks locations that are closest to each another?

---

### Main Findings
#### 1. What are the top 15 countries with the most Starbucks stores?
![](https://github.com/hollyjanedalton/final_ironhack_project/blob/main/starbucks_count.png)

Answer: US takes the lead by far, and Canada and Mexico, the other two North American countries, are also in the top 7. 

#### 2. Where in the world do the earliest Starbucks locations open, and at what time? (Excluding licensed stores, such as those inside hospitals, train stations, airports, etc.)

Answer: 38 Starbucks stores open at 3:30 AM in the US

![](https://github.com/hollyjanedalton/final_ironhack_project/blob/main/earliest_starbucks.png)
**In the map above, green dots represent stores that open at 3:30 AM. 

#### 3. Where in the world are the two Starbucks locations closest in proximity to one another?
Answer: In Jakarta, Indonesia 🇮🇩 there are two stores that are less than 80 meters apart, or less than a 2-minute walk! 
![](https://github.com/hollyjanedalton/final_ironhack_project/blob/main/two_closest_cafes.png)

---

### Conclusions

1. There are WAY more Starbucks cafes in the U.S. than in any other country, by far. But, if we take into consideration population size, Kuwait, Canada, the Bahamas, and South Korea are not far behind. And, if we consider country geographical size, Singapore actually has a higher density of Starbucks cafes than the U.S, for every 100 km squared.
2. The U.S. is the ONLY country that has Starbucks coffeehouses opening at 3:30AM every morning. 
3. The 2 closest Starbucks in the world are NOT in the US, but in Jakarta, Indonesia (less than 80 meters apart) 

## So, Are North Americans Really Starbucks' #1 Fans?
### YES, but countries that are densely populated, geographically small and have modern economies with relatively high GDP per capita (Singapore, Kuwait, South Korea, Hong Kong, etc. ) are also big Starbucks fans. 

Countries in regions of the world like Europe, Africa, and South America in general do not have Starbucks-crazed cultures.

---

### Data: 16 location features of over 28,000 Starbucks Locations
#### Here's a quick look at the raw dataset 
<img src="./small_data_photo.png">

#### I eliminated many of the features and focused my analysis on: 
- Country 
- City
- Ownership type (Company owned, Licensed, Joint Venture or Franchise)
- Hours of operation 
- Latitude and Longitude (Accurate up to 6 decimal points) 

#### I later web scraped and added to the data:
- 2021 Country population
- Country area
- Country population density (km²)

---

### Process
1. Import Starbucks dataset from Kaggle to python and complete exploratory data analysis
2. Data cleaning: 
      - Handle NaNs, duplicates and empty cells, outliers
      - Standardize features names
      - Use regex to reformat opening hours into readable form 
      - Decide columns and rows to drop
3. Web scrape population data from https://worldpopulationreview.com
4. Create new dataset with population and Starbucks data and clean the dataset
5. Build function to compare Latitude and Longitude of every Starbucks to find the two that are closest to each other (this was quite advanced and I had help from instructor, Jan Molendijk) 
6. Fill 18% NaNs in the "Hours of Operation" column: 
    - Use the "Hours of Operation" of the  literal "nearest neighbor" found with the #5 Function
7. Data Visualizations in Tableau
     - Map of Starbucks stores that open the earliest
     - Bar chart of countries with most Starbucks (top 15)
     - Bar chart of Starbucks per capita
     - Map of world showing country with most Starbucks per area (density)
     - Map of world showing country with 2 Starbucks that are closest to each other (using Lat/Long)
8. Prepare presentation on slides.com with results 
9. 9-minute presentation with discussion afterwards with 20+ Ironhack colleagues 
