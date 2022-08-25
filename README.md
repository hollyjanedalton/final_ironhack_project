# Analysis of Starbucks Locations 

## Mapping Starbucks locations with latitude/longitude and population data

[Click for recording of final presentation](https://ironhack.zoom.us/rec/play/z_KuzP88l79dzVBAtHaR-vPE4Xi4xUGUU-C3D948G81Z7jHR7GCBa8oip2yDNDrNwbnBrP9AWwVZ6sM9.WElypAcnuo2-6udI?startTime=1660305720000&_x_zm_rtaid=v-1r2qOaSt-VQG_GldUWIA.1660487182977.ee234b4949979eb90f4b2d2092f0085f&_x_zm_rhtaid=21)

[Click to view presentation slides](https://slides.com/hollydalton/deck-5b0977/fullscreen)

### Objective: Use web scraped Starbucks store location data and population data to answer 3 questions:
1. Geographically, how are Starbucks locations spread across the world?
2. Where does the earliest Starbucks location open, and at what time?
3. Where are the 2 Starbucks locations that are closest to each other and how close are they to each other?


#### Data: The data set consists of 14 demographic features on 18,000 current bank customers:
storeNumber	countryCode	ownershipTypeCode	schedule	slug	latitude	longitude	streetAddressLine1	streetAddressLine2	streetAddressLine3	city	countrySubdivisionCode	postalCode	currentTimeOffset	windowsTimeZoneId	olsonTimeZoneId


- Store Number: A sequential number assigned to each store.
- Country Code: 2-letter code indicating in which country the store is located 
- Ownership type: The type of reward program offered for the card.
- Hours of operation: Letter or postcard.
- Slug: Low, Medium or High.
- Latitude: How many non-credit-card accounts are held by the customer.
- Street address line 1: Does the customer have overdraft protection on their checking account(s) (Yes or No).
- Street address line 2: Low, Medium or High.
- Street address line 3: The number of credit cards held at the bank.
- City: The number of homes owned by the customer.
- Country subdivision code: Number of individuals in the family.
- Postal Code: Does the customer own their home? (Yes or No).
- Current time offset: Average account balance (across all accounts over time). Q1, Q2, Q3 and Q4
- Windows timezone ID: Average balance for each quarter in the last year
- Olson timezone ID: 
