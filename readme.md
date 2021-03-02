# Ford GoBike Data Analysis
## by Fletcher Sarip


## Dataset

The dataset contains the bike usage of Ford GoBike on February 2019. The data consists of 183412 bike usage records in the dataset with 14 features, which are bike rent duration, start and end time, start and end station name and location, bike ID, user type, user birth year, and user gender.

## Summary of Findings

It is observed that the bike rent duration distribution is highly right-skewed, hence I needed to transform the duration to be in log scale. Once it is transformed to log scale, it is found that the duration (under log scale) is normally distributed. The average bike rent duration is around 516 seconds, with actual values ranging from 60 seconds up to almost 24 hours.

There are much more demands from subscribers than from customers, where 89% of the bike demands are from subscribers, while 11% are from customers. However, to my surprise, customers tend to rent the bike for longer duration than subscribers, where the average rent duration for customers is 842 seconds, while for subscribers it is 486 seconds. This trend on customers renting for longer duration than subscribers is observed consistently regardless of user age, gender, station location, and booking time.

The age of the users range from 17 years up to 92 years old, where most users are around 30 years old, and older users are observed more than younger users (the age distribution is right-skewed). It is observed that users in the 60s age category tend to rent the bike for longer duration compared to the other age categories. It is also found that generally users below 60 years old tend rent the bike for duration ranging from 100 seconds up to 3000 seconds (excluding outliers). Users above 60 years old tend to rent the bike for shorter duration. Above 80 years old, the users in general have much lower rent duration, ranging from 60 to 1000 seconds. Thus, in general, older users tend to rent the bike for shorter duration than younger users.

It is found that here is much higher percentage of male than female users, with "other" gender being the lowest. 71% are males, 22% are females, 4.5% are not given, and 2% are "other" gender. However, interestingly females and "other" gender users in general rent the bike for around 70 seconds longer than male users, with the "other" gender average duration slightly longer than females average duration. Also, this relationship holds regardless of the user age, i.e. female users of all age tend to rent the bike for longer duration than male users of all age.

The bike stations are observed to be clustered into 4 regions, which I named as NorthWest, NorthMiddle, MiddleEast, and SouthEast (the first syllable correspond to latitude-wise cluster and the second syllable correspond to longitude-wise cluster). It is observed that NorthWest region has the highest demand, followed by NorthMiddle, SouthEast, and lastly MiddleEast being the lowest. For the bike rent duration, it is found that MiddleEast tend to have the longest rent duration, generally ranging from 100 seconds to 66 minutes, followed by NorthWest region generally ranging from 100 seconds to 50 mintues. NorthMiddle region has similar distribution with NorthWest with slightly shorter duration, generally ranging from 100 seconds to 40 minutes. SouthEast region tend to have the shortest rent duration, generally ranging from 100 seconds to 30 minutes.

With respect to booking time, it is observed that weekdays have higher demands than weekends. On the contrary however, the rent duration is generally longer during the weekends than during the weekdays, where during the weekend the duration can generally go up to around 80 minutes, while on weekdays the duration is generally only up to 50 minutes. With respect to location and day of week, on average the bike rent duration is the longest during the weekend in MiddleEast region (consistent with the finding in the previous paragraph), being on average around 15 minutes, roughly 5 minutes longer than the average duration of the other regions during the weekend.

Also, on daily basis, there are peak demand hours at 08:00 and 17:00. The rent duration tend to be longer during middle of the day, around 11:00 to 15:00, and during midnight around 00:00 to 02:00, where during this time period the rent duration can generally go up to 66 minutes, while on average during the whole day the rent duration can only generally go up to 50 minutes. It is suspected that the long duration in the midnight might be due to the bike being rented overnight and only returned in the morning.

## Key Insights for Presentation

For the presentation, I focus on presenting the distribution of demands and rent durations with respect to the user demography, location, and time. I will represent the demand level with the data count. As for location and time, I used the start location and start time, with the reason that it is the start location and time that influences bike rent demand.

In the presentation, I started with presenting the distribution of rent durations. Then I proceeded with presenting the clustered regions of the bike stations, where the bike stations can be clustered into 4 distinct regions. Afterward, I proceed with presenting the distribution of demand levels and rent durations with respect to user demography, location and time, both in bivariate and multivariate manners. I've made sure to present the plots with as high data-ink ratio as possible.