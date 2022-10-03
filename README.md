# Vacation search using Gmaps. 

## Overview of Project
Planmytrip is a top travel technology company that specializes in internet related services in the hotel and lodging industry. Jack is the head of analysis for the user interface team. He's asked me to help to collect and present data for customers via the search page, which they will then filter based on their preferred travel criteria in order to find their ideal hotel, anywhere in the world. Using the Google Maps Directions API we are doing below technical analyses. 

* Retrieval of Weather Data

* Create a Customer Travel Destinations Map

* Create a Travel Itinerary Map

###  Challenges
Retrieving weather data for 2000 cities is a bit challenging. Data retrieval takes a long time (~15 min) because the sleep timer which is 60.    
Encountered different errors while executing the code. To mitigate this, I used the exception handling mechanism. Skipped the city if an error is experienced. 
 
### Analysis Results: 
Weather py database contains 745 cities from the size of 2000 latitude / longitude pairs.

![Screen Shot 2022-10-02 at 11 33 21 PM](https://user-images.githubusercontent.com/44387918/193519386-d073ea64-ee1f-4b0c-9c0b-36b476dd793f.png)

Filtered preferred cities using minimum and maximum temperature criteria. Minimum is 50 and Maximum is 80 in my case. 

![Screen Shot 2022-10-02 at 11 39 19 PM](https://user-images.githubusercontent.com/44387918/193519435-22bb13b5-2fa2-49da-be4a-93e7b0464422.png)

Retrieved clean hotel data by dropping null values. Below is the marker layer map based on location and maximum temperature.  

![Screen Shot 2022-10-02 at 7 04 04 PM](https://user-images.githubusercontent.com/44387918/193519676-821612be-135b-421f-9be2-ee12a8f31826.png)

![Screen Shot 2022-10-02 at 11 43 50 PM](https://user-images.githubusercontent.com/44387918/193519584-153ca33d-b3ac-4117-9c71-4ab4bb789254.png)

Created directions layer map using the vacation start and end points along with waypoints and travel mode. 

![Screen Shot 2022-10-02 at 11 46 07 PM](https://user-images.githubusercontent.com/44387918/193519621-a3019a8f-057f-4603-9e79-b1438ab4a7ae.png)

## Conclusion
Since the data is random, I am not able to analyze the accuracy of information. Api’s are powerful tool to analyze the data in various ways. Gmaps library is very useful and well documented. Especially, places API has a robust features, we can find a places, nearby search, details and photos etc. 
