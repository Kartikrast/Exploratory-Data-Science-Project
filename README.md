# Airbnb Bookings Analysis
![_Blue   Navy Modern Business Facebook Cover](https://github.com/user-attachments/assets/11ad84f6-2bd5-439c-97f8-f69d86c07eef)

# Project Type
**Exploratory Data Analysis**

**Contribution:** Individual

**Project Video Link:** https://www.linkedin.com/posts/kartikeyrastogi162_dataanalysis-exploratorydataanalysis-businessanalysis-activity-7217867182683095041-kPm0?utm_source=share&utm_medium=member_desktop

# Project Summary
This project involves performing an analysis on the data having around 49000 observations. The objective is to seek-out meaningful insights from this data to provide crucial information to the management and the stakeholders to make decisions on what can be done to expand or improve the business, eventually leading to the growth of the business. This project will identify the patterns that are being formed in these observations and based on those patterns some suggestions can be taken in consideration. This analysis will help not only the guests to make better choices but it will also be helping the hosts, so that they may make the required changes in order to grow their business.
As we are provided with information like:-
- Listing Counts
- Data Distributed as per specific neighborhood groups
- Prices
- Reviews data
- Room Type Preference

Using this information we will be able to seek insights like:-
- Preference of the guests for their hosts
- Room-Type preference
- Prefered Price range
- Most preferred neighborhood

We will also be able to create a filter system for our guests to provide them with the listings as per their budget and other preferences, we will be able to rank our hosts as per their ability to match the guests requirement, this way we will be targeting customers with specific needs and we will be fulfilling those needs, which will eventually enhance customer experience, and they will be getting utmost satisfaction when all of their needs will be fulfilled.
We will also be able to provide our hosts with the information on what they can change or improve so that they can get more attention and also they will be able to fulfill the needs of their guests.

Majorly we will be doing data wrangling using **PANDAS** to frame this data more clearly and seek out meaningful information that can be used to analyze the requirements and the preference of the guests.
There might also be a need to create other data frames so that information can be stored separately and can be accessed whenever needed.

For computations and calculations on the numerical data we will be using **NUMPY** so that we can seek insights mainly for ranking purposes. Numpy will be helping us to create required arrays so that the data can be stored and accessed in a systematic manner.

In order to simplify and study the results and the analysis more efficiently, the optimum presentation of the analysis is a must, which makes it easier for the stakeholders to understand the results of the analysis and make informed decisions. In order to achieve this we will be using Matplotlib and Seaborn for data visualization and for the presentation of the insights.

Now coming onto what I will be learning from this project, as this is a real life situation where I will have to do some research on how things really work in this field I will be getting the knowledge of the working model of this business, along with this I will get an idea on how do we need to think and create solutions for the problems, however identifying problems in any statement is also a skill in itself, this project will also help me to polish those skills as well, talking about data science, I will be learning the optimum utilization of the libraries which will help me to learn how to use the methods provided in the best way possible, I will also be working on critical thinking on how to apply some provided complex concepts on this given data so as to make it more meaningful as if it is telling a story.

This data analysis project will help me improve my knowledge and skills and also my understanding of the real time complexities.

# Business Objective
The business objective of this project is to identify opportuinites of improvements and also to derive patterns and insights of customer's preference which will ultimately help us in achieving customer satisfaction.

# All about the Dataset
The Airbnb NYC 2019 Dataset has:-
Rows = 48895
Columns = 16

We can see the division of Categorical and Numerical values in our dataset, We can see:-

3 columns have float64 data values (Numerical)
7 columns have int64 data type values (Numerical)
6 columns have object data type values (Categorical)

The dataset contains both numerical and categorical data.

The primary key of our dataset is the "id" column, having a unique IDs for the hotel names.

Here is the list of columns:-
['id', 'name', 'host_id', 'host_name', 'neighbourhood_group',
       'neighbourhood', 'latitude', 'longitude', 'room_type', 'price',
       'minimum_nights', 'number_of_reviews', 'last_review',
       'reviews_per_month', 'calculated_host_listings_count',
       'availability_365']

This dataset had no exact duplicated values, however in the name column there were 998 rows that were duplicates.
Where all the values were almost the same, except for the prices, there might be a chances that the prices were altered with time as per the market condition however the hotel was the same.

To handle these values we sorted our dataframe on the basis of latest entries, for which we needed a timestamp in our dataset.
In our dataset we were able to use the 'last_review' column as the timestamp for our dataset.

After doing few operation we were successfully able to handle our duplicated values.

These are columns that majorly has the null values:-
- last_review = 10052
- reviews_per_month = 10052

As the date column was missing values we replaced the NA values with the latest date present in our dataset, so that the time stamp could be efficient.

We are also missing few "Names" as well as "Host Names":-
- name = 16
- host_name = 21

We have now successfully formatted our dataframe and it is now ready for data wrangling.

# Understanding Variables
There are basically 3 types of variables according to their roles:-

- Numerical Variables: These variables represent quantitative data and can be further categorized into:-
  
  - Continuous Variables: These variables can take any value within the given number of range.
  - Discrete Variables: These variables are having a specific value and are related to a specific identity.

- Categorical Variables: These variables represent qualitative data and can be further categorized into:-
  - Nominal Variables: These variables are random and they do not follow any order or ranking.
  - Ordinal Variables: These variables are according to an order they can be ranked as well.

- Time Variables: These variables are basically date and time variables having a timestamp.

  # Manipulations and wrangling performed
  This dataset was having good amount of well distributed information, which was a plus point for our study. As this dataset if of Airbnb, the locations play a very crucial role in these values and the inforamtion was distributed well as per the locations and their respective areas.

We have done number of manipulations to seek information which can be beneficial for the stake holders to make decisions for the business, not only that our hosts will also get good idea about the preferences of their customers, as we promised in our agenda.

We divided the complete manipulation into 2 major parts, as per the features and the relationships, so that we can draw insights accordingly.

These are the manipulations we followed:-

- Created a new price range column: As this columns will help us to categorize the price distribution and to simplify the judgement for us to get an idea of the budget of our customer, we have tried to keep it as precise as possible.

- Sorted the dataset as per price: As the data wasn't sorted and was not having any significance regaring any value, we sorted it as per the pricing, keep the most expensive ones on the top.

- We filtered the data so that it becomes simple and easy to understand(less chaotic) for us to work only with those columns that are required for the data analysis and feature engineering.

- Divided the data accoring to the categorical groups to derive insights accordingly, it helped us to identify the outcomes in a structed manner with respect to the considered groups, it provided us with more specific information about the different groups we created so that we can identify insights for each group individually. These are the diferent groups we created and worked with:-
  
  - Created Nighbourhood Group: This group helped us to get an idea of which neighbourhood is the most prefered one in all of the neighbourhoods.

  - Created room type groups: This group helped us to identify which room type is the most prefered by our customers.

  - Created Neighbourhood area groups: This group helped us to identify which is the most prefered area within the neighbourhoods.


We also worked on few of the relationships that helped us in few comparisons that will help our stake holders to make decisions accordingly. These are the relationships we worked with:-

- Relationship: Price vs. Room Type
  - Checked the distribution of prices for different room types.
  - Determined which room type is having the most expensive price distribution.

- Relationship: Reviews per Month vs. Room Type
  - Compared the distribution of reviews per month for different room types.
  -  Explored the level of engagement and satisfaction of our customers as per different room types.

- Relationship: Price vs. Neighbourhood
  - Compared the distribution of prices across different neighbourhoods.
  - Identified neighbourhoods with higher or lower average prices and explored price variations as per the areas.

These are the manipulations that we did in order to derive useful information so that it can contribute into the growth of our business and also the busniness of our hosts, and ultimately grow and improve tavelling experience for our customers.

The specifilly derived insights will be mentioned with the visualisations so that it would be better to understand and visualize at the same time.

# Few of the tabular Outcome from the insights derived in Excel
- **Neighbourhood Data**
  
  ![image](https://github.com/user-attachments/assets/b4c14660-aef4-4813-b451-006641cb9612)

- **Neighbourhood Groups Data**
  
  ![image](https://github.com/user-attachments/assets/51c71510-b7e3-439e-9b27-015a566e4998)

- **Most Prefered Price-Range**
  
  ![image](https://github.com/user-attachments/assets/6a1c18c4-29dd-4e32-9db5-1a262bb2da88)

- **Hosts with most Listings**
  
  ![image](https://github.com/user-attachments/assets/7c3652d4-4ff2-437d-b394-ecd1fa3dc575)

- **Room Types Data**

  ![image](https://github.com/user-attachments/assets/bb68a4a5-d048-468f-8922-776e8731b27a)

# Dashboard First Look

![image](https://github.com/user-attachments/assets/98351e85-26f3-4454-a474-02f9ff9f806f)


# Solution to the Business Objective
Coming up to the solution of our business objective, we have throughly studied the whole data set and drawn some conclusions based on that, here are all the pointers we can take into consideration.

- 0-300 is the most prefered price range, which gives us a clear idea on what basis we will have to create our pricing.
- Entire home/apt	being the most prefered room type makes it obvious that customers are very much concerned about their privacy and safety, we can create more relevant policies regarding their safety and privacy, ulimately resulting in gaining their trust and creating goodwill.
- We know that the most prefered area is the Financial District which is in the Manhattan Neighbourhood Group, hence we can create recommendations as per the pricing and area preferrences.
- The most reviews are also given to the same area itself we can take into consideration those points which proved to be the most satisfying for our customers so that we can make such changes in the other neighbourhoods, if possible, whcih will result in getting us more business in the other areas as well.
- I personally feel that this dataset should have one more column as per the occupation of the customer, it will create different groups of our customers based upon their occupation, which will help us to determine the preference of people coming from different sectors and we can identify which group of customers prefers which kind of accomodations.
- This dataset also gave us a good idea on the budget of the majority of our consumer market, and now just that we were able to see the ratio of prefered pricing.
- We were clearly able to see where most of our business lies and which consumer group creates the most of the business for us, we can make improvements in those and not just that we can also focus on the other sectors as well so that we can expand our business even more.

# Conclusion
The conclusion of this complete EDA project is simple and crisp, we have enough data to see what is liked by our customers and what is it that they are demanding as is is clear that around 90% of our business is saturated into one side whether it is the area preference or pricing, we can use that information to check what works for our customers and make those changes in other areas as well.

# Thank You
