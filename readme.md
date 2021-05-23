
# Ford GoBike System Exploration

## Dataset

The dataset has information regarding 183,215 bike trips of Ford GoBike System, recorded in February, 2019. This dataset includes, bike_id, user details(age, gender), time of the trip(start and end, with date), location of the starting and ending point. I have downloaded the data from this url : https://s3.amazonaws.com/fordgobike-data/index.html and licensed by https://assets.fordgobike.com/data-license-agreement.html

## Summary of Findings

I have divided the exploration in 3 parts :

**Univariate Exploration** - 
Majority of the riders are male(71.2%), with less than a quarter female(22.2%). A log transformation is needed for duration of the trip as it was very left skewed, with majority of rides being short. 90% of the trips are less than 20 minutes long. Of which, 3 quarters are shorter than 13 minutes.
Bimodal distribution is observed when plotting a graph of average trip count during the whole day, with a peak at (7-9)am in the morning and second at (4-6)pm in the evening.Bike traffic on weekdays is double compaired to the weekends.
<br><br>

**Bivariate Exploration** : <br>
This type of exploration mainly deals in relationship between two features. 

- Weekdays Vs Weekends <br>
Average Duration (min) of the trip in Weekends is higher than weekdays.
Average Speed (Kmph) of the bikes during Weekdays is higher than weekends
Average Distance (Km) covered in the Weekdays is higher than weekends. <br>

- Subscribers Vs Non-Subscribers (customers).<br>
The Subscriber average trip duration is less than half of that of the customers. Subscribed riders have shorter variance/range of duration. They seem to have fixed time/path, with less variation. Subscribers travels faster than Customers. Subscribers also have a more consistent speed range.It seems subscribers are more experienced and take the same route everyday (don't have enough data to back that).<br>
- Average Bike speed at different times of the day.<br>
Maximum speed is between Morning 4am - 9am. Reaches the peak at 6 am and traffic start increasing and speed gets down. It hit the lowest point at afternoon, (12-3)pm.After 4pm the average speed is almost constant,with slight increase, till midnight.<br>
<br>

**Multivariate Exploration**: <br>
Here are the finding:<br>
- Subscribers are faster than Customers, (Average Customer speed) : 8.5 Kmph, while (Average Subscriber Speed) : 11.05 Kmph.
- In both male and female we can see the trends that the speed declines with age. Males are slightly faster than both the groups (female and others).
- Older people (60 +) are more inclined to be a subscriber of the service (61% more subscriber than it should be over the age of 60).
- The number of trips by subscribers decreased by approximately a factor of half in weekends compared to weekdays, but for customers there is almost no difference. Thursday is the most popular day for both subscribers and customers to head out for a trip.
- During the weekdays, most number of trips are during morning and evening., whereas during the weekends, most number of trips happen during the afternoon and evening.

## Key Insights for Presentation

For the presentation I will be focusing on three aspects, Rider(age and gender, user type) , Time (period, hour of the day) and Trip(distance, duration and speed). I will show the relationship between time of the day and the number of trip, it's average speed and duration.

After that, I will put the spotlight on the user type and how it affects other key aspects of the trip, including duration and speed. I will also show how the age and gender can have an affect on the trip. I will keep in mind to have clean plots, with very high data-ink ratio and no chart junks, by using the best practices.  


### Resources:
For this project, help is taken from following sources:
- Udacity (Asking Mentors, Code from the lesson itself)
- Websites:
    - https://stackoverflow.com/
    - https://seaborn.pydata.org/
    - https://matplotlib.org/
    - https://www.w3schools.com/python/

