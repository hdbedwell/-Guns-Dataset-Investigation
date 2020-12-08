# -Guns-Dataset-Investigation
Gun permits and overall gun transaction trends.

The data comes from the FBI's National Instant Criminal Background Check System. The NICS is used to determine whether a prospective buyer is eligible to buy firearms or explosives. Gun shops call into this system to ensure that each customer does not have a criminal record or isn’t otherwise ineligible to make a purchase. The data has been supplemented with state level data from census.gov. I will be investigating the following questions:

Which states have had the greatest increase in gun permits between 1999 and 2016? 
What is the overall trend of gun transactions between 1999 and 2016?

Introduction
This analysis will explore which states have had the greatest increase in permits between 1999 and 2016. In addition, this analysis will explore the overall trends in gun trascations between 1999 and 2016.

See notebook.

Conclusions

Using data from the FBI's National Instant Criminal Background Check System, I examined:
   Which states had the greatest increase in gun permits between 1999 and 2016?
   The overall trend of gun transactions between 1999 and 2016?

After an inital assessment of the data, I determined that I needed to address missing values using the fillna function. I also, needed to create two new columns to separate the month and year from the month column so that I could look at the data by year rather than by month/year. Since this was central to my investigation< i also had to confirm that I had full year data for each of the years I was exploring. As a result of finding that 1998 only contained data for two months and 2017 only contained data for the first nine months, but all other years had data for all twelve months, I decided to compare data between 1999 and 2016.

I determined the total number of permits issued for each yer and found the difference for each state. I then sorted the permit difference by state and found the top ten states with the greatest increase in permits.

In conclusion, the state with the greatest increase in permits between 1999 and 2016 was Kentucky, with an increase of over 3 million permits during this time period. At a distant second was Indiana followed by California, both with an increase of over 900,000 permits and finally Illinois. Florida, Texas, Pennsylvania, Minnesota, Alabama, and Washington round out the top 10 states with the greatest increase in permits during this time.

Interestingly, on June 27, 2019, Kentucky "became the 16th state to allow gun owners to carry concealed firearms in public without training or a permit." (Source: https://www.thetrace.org/rounds/daily-bulletin- kentucky-permitless-carry-nics-notification/ (https://www.thetrace.org/rounds/daily-bulletin-kentucky- permitless-carry-nics-notification/))

Next, I looked at total gun transactions across states during this same time period. I found the total number of gun trasnactions per year and then plotted the transactions against year to see if there were any noticable trends. The overall trend in total gun transactions during this time shows a steady increase from under one million annually in 1999 to over 2.5 million transactions in 2016.

LIMITATIONS: One of the most notable limitation of this dataset is that it is not accompanied by data notes, a data dictionary, or business rules to explain the data. Since we are provided counts by state, by month/year, for each metric, we are not able to dtermine, based on the data how long permits are good for by state and how often permits are required to be renewed. If one state requires annual renewals and another state only requires renewals every 5 years, we may observe more trasnsactions in the data in the state that requires annual renewals. We also can not dtermine from the data which states and how often permit checks are performed or required.

Another major limitation of the data is determining which variables may help us determine how many guns are out in the coummunity versus those that have been redeemed, returned to seller, pre-pawned, or are being held by renters. Further, how many rental guns have never been returned? We would definitely need additonal information to conduct a deeper and more meaningful analysis of this data.
