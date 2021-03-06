# Academic Project: Demystifying-Customer-Satisfaction-for-a-Hotel

## Syracuse University Coursework: Demystifying Customer Satisfaction for a Hotel   (Jan,2018 - May,2018) 
MS Data Science Projects and coursework @ Syracuse University 
                                                                  
- Tools & Techniques: R, Linear Regression, SVM, Naïve Bayes, Association Rules
- Analyzed data patterns in (~1.7 M) customer survey responses for a multinational hotel chain & produced actionable insights through predictive analysis for hotel’s performance across the globe by modelling key factors (KPI drivers) impacting customer's likelihood to recommend & improving Net Promoter Score 


#### Agenda

### I. Data and Key Performance Indices provided

### II. Descriptive Analytics and understanding patterns

### III. Understanding Current Performance

### IV. Approach

### V. Key factors impacting NPS across the board

### VI. Factors Impacting NPS for specific population groups

### VII.Conclusion



#### Executive Summary

##### › We got data for 1 year across multiple categories including:

##### » Customer Aspects: Contained customer demographics and profile information such as Age, Gender

##### » Booking Factors Information: Contained data such as check-in date, length of stay and Type of room

##### » Hotel Details: Hotel characteristics like the Hyatt Corporation brand, location, and available amenities

##### » Customer feedback: detailed customer feedback on different aspects of the service, along with customer's eventual Likelihood to

Recommend rating and NPS_Type

##### › The data was viewed from multiple angles and based on the above data we did extensive analysis of Hyatt’s Performance and customers’

feedback

##### › Using descriptive and advanced data analysis techniques we have been able to identify key levers for improving customer satisfaction and have

impact on the NPS KPI

##### › The identified factors have been proved correct and powerful enough to accurately predict NPS score in 80%+ cases

##### › With these insights Hyatt group will be able to get actionable insights on how to improve NPS


#### I. Data and Key Performance Metrics

###### Given feedback on multiple columns, Based on feedback data , three key metrics available

**Understanding the Available Data**


#### II. Understanding Current Performance

##### Analysis of Countries

**BQ 1.** How is Hyatt doing overall in general? In the Hyatt dataset provided, after cleaning, what is the count or spread of customers worldwide with
respect to different Purpose of Visit and the three NPS types?

**Population by Country ACTION POINTS**

- Observations:
- United States has the highest number of reservations which accounted for 81% percentage of
total reservations. Observations in many other countries are significantly less
- There is scope for improvement in general for Hyatt Corporation
- United States brings in most business to Hyatt group and there is scope for improving
performance as its NPS score is 57% and is lower than average NPS score of 61%.
- Further, Hyatt has a good opportunity to analyze expanding its presence in countries outside the
United States, as currently it has very low presence outside United States including countries
which are bigger and more populous than USA (India and China).
- Key Observations and Insights:
- Average NPS across all countries has been

found to be 60.69% (average LTR 8.76)

- Poland is having the highest NPS 91% (average

LTR of 9.64)

- Jamaica having the lowest NPS -16% (average

LTR of 6.22)

```
Country
Name
LTR Population NPS
Poland 9.65 48 91.
Ukraine 9.48 378 88.
Russia 9.36 1887 80.
Greece 9.29 369 79.
... ... ... ...
United
States 8.65^744959 57.
... ... ... ...
Philippines 8.20 1239 38.
France 7.99 10241 34.
Guam 7.90 1503 27.
Jamaica 6.23 92 - 16.
```

#### III. Understanding Current Performance

##### Analysis of States of the USA

**ACTION POINTS**

- In United States, for fastest
gains, Hyatt must of focus on
states of Colorado, Virginia
and Florida as their average
LTR is very close to 9 and
they are amongst the top
most contributors by
reservation counts after
California.
- Bigger states of California
and Texas have highest
reservation count of 114,
- the State of ‘California’ as it
provided the most
population for doing data
analysis.


###### III. Understanding Current Performance

#### Analysis of Brands

**BQ 2.** What is the comparison between Hyatt Hotels sister
brands and their effect on NPS?

**ACTION POINTS**

- Hyatt Regency had the least NPS
score when compared to other
sister brands.
- Also, working on higher
population data ensured a
robust analysis.
- Further working on Hyatt
Regency allowed to focus on a
small region and ensured
capturing of regional
phenomena well.
- Analysis of reservation counts
for each brand within California
showed that Hyatt Regency
seems to have the most data
and maximum no. of
reservations of each type,
making it the ideal brand to
focus on


#### Some more Descriptive Analytics before we move to Validation


#### IV. Approach going forward

###### Data Cleaning Preprocessing Data Exploration and Analysis

###### Model Development for

###### Advanced Insights

##### Insight Generation

- Initialtotalcolumnsinthegiven
12 monthsofdatasets: 237
- Columns retained: 40
- Rows read: 15,711,552 obs. of
40 variables
- comprehensive identification
of missing values. All blank cells
were converted to the value NA
to ensure all missing values are
marked as NA
- Columns having more than 90%
missing values were dropped
- Columns which didn’t have any
relevance to LTR or NPS_Type
were dropped
- All rows having missing
countries were removed
- **Final Clean Data: 924378 obs. of 40**
**variables**
- Linear Regression
- Support Vector Machines
- Association Rules
- Boruta Random Forest
- Customer Service
- Hotel Condition
- Guest Room
are the most powerful variables
affecting NPS Score and
Likelihood_to_recommend.
- Other local patterns

**Process Followed**

```
Data across all geographies and
brands was first analyzed in depth,
and then it was iteratively sliced
into subparts that had the highest
data volume at each level.
Hypothesis was that focusing on
parts having most data will allow
us to generate analysis based on
widercustomer behavior patterns.
In United States, California had the
largest dataset, because California
also has the largest population.
Similarly, Hyatt Regency was chosen
as the next dataset as it was found
to have the highest observations.
```

#### V. Key Factors Impacting NPS Across the Board

**BQ 3.** How is guest feedback related to NPS & how do these numerical factors impact on customer's likelihood to recommend? How can NPSScore be
improved with these?

**Correlation Model Details**

**FACTORS IDENTIFIED**

- Overall Key levers for NPS seem
to be same across the board
for all Hyatt Regencycustomer
ü **Customer_SVC_H:** Quality of
customer service metric;
value on a 1 to 10 scale
ü **Condition_Hotel_H:**
Condition of hotel metric;
value on a 1 to 10 scale
ü **Guest_Room_H:** Guest
room satisfaction metric;
value on a 1 to 10 scale
- These patterns in full data
get sometimes mixed and
hence might look like
noise , Hence in order to
get finer local patterns we,
divided the data into
specific Business and
Leisure population.


#### BusinessTraveler

**BQ 4.** Which of factors related to hotel amenities across different purpose of visits (Business and Leisure) are important in determining NPS score? How to
improve NPS Score using these factors?

**Business Promoter**

**Business Detractor**

**FACTORS IDENTIFIED**

- Beyond the three common categories of Guest Room, Condition of Hotel and Customer service which are universally true for making a customer to be promoter, we also
found that business customers value Tranquility, Good internet connection and presence of Business centers and Convention centers at Hyatt Regency in California.
- Hence, to increase Promoters, we recommend to Hyatt that they put high effort in providing guests with Tranquility and internet satisfactioninhotelssothatbusiness
meetingsflowinthebestwaypossibleasmeetingsathotels need to be peaceful and adequate infrastructure including high speed internet connection will boost business
conversations and outcomes. This can be done by providing rooms to business travelers **onhigherfloorsandawayfromcommonlobbiesandothernoisyspaces**.
- Apartfromthis Hyatt must also focus on constructing indoor pools and providing minibars as absence of these factorsmightleadtoevenworseoverallsatisfactionleadingto
lowNPS.

**Observations & Insights:**


#### Leisure Traveler

**Observations and Insights:**

- Leisure Promotor travelers also concentrate on presence of outdoor pool, spa, great check in experience and caring staff.
- Other parameters prove that leisure customers highly value personal experience with the hotel, like a good check in and caring staff.
- To increase promoter counts amongst leisure travelers we recommend Hyatt focuses on **ensuring best customer service at check in and**
**prompt and empathetic service staff.** The detractor patterns are highly correlated to patterns of promoters. The top parameters that lead
to Leisure visit detractors are low tranquility, lack of caring staff and lack of amenities like Spa_PL and LimoService_PL.

**Leisure Promoter Leisure Detractor**


#### Consumer Demographic

**BQ 5.** What is the relationship of various booking factors on NPS? How can it be improved?

**Booking Factors Promoters**

**Booking Factors Detractors**

**Observations and Insights:**

- Younger parent(s), especially if single, seem to have a harder time at the hotel and give less ratings when with 2 children, especially
when compared with older parents who are travelling together.
- We recommend making the hotel friendlier and helping to needs of young parents, by providing services **like play area/care centers**
**and staff for kids.**
- We also recommend providing **family discounts to parents visiting the hotel**.

**FACTORS IDENTIFIED**


#### Conclusion

- Total,thisprojectused **over 3 DataScienceanalyticsmodels** – Linearregression,AssociationRules,SupportVectorMachinesandBorutaandgeneratedfollowinginsights.Also,thedata
wasviewedfrommultipleangles,andthebusinessquestionsquotedbeforehavingledtogenerationoftrendsandpatternswhichwerevalidatedthroughmodelling.Hencethesetangible
andactionablestepscanbeusedbyHyattCorporationCEOtoimproveNPSScore.
- Throughouranalyticstechniques,OverallKeyleversforNPSseemtobe **UNIVERSAL** acrosstheboardforallHyattRegencycustomers:

```
ü Customer_SVC_H: Quality of customer service metric; value on a 1 to 10 scale
ü Condition_Hotel_H: Condition of hotel metric; value on a 1 to 10 scale
ü Guest_Room_H: Guest room satisfaction metric; value on a 1 to 10 scale
```
- OnceagainlikeBoruta,AssociationRulesalsoprovedourassumptionandfactorshavingthehighestvariableimportancewere:(inthisorder)
- Customer_SVC_H
- Guest_Room_H
- Condition_Hotel_H
- Staff_Cared_H
- Tranquility_H
- Check_In_H
- Internet_Sat_H
- LimoService_PL
- Spa_PL
- The local patterns in full data get sometimes are mixed and hence might look like noise , Hence in order to get finer local patterns we, divided the data into specific Business and
Leisure population. Having figured out that in order to generate patterns and association between the above important factors, Association Rules mining was performed which will
helped predictingrulesthattellexactlywhatis thepatternbetweenthesefactors.

**By understanding and improving on the recommendations, Hyatt will be able to increase %
Promoters and decrease % Detractors and this will help raise its overallNPS Score.**




