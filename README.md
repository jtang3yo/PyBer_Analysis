# PyBer_Analysis
## Overview 
1. Background 
  V. Isualize has given you and Omar a brand-new assignment. Using your Python skills and knowledge of Pandas, you’ll create a summary DataFrame of the ride-sharing data by city type. Then, using Pandas and Matplotlib, you’ll create a multiple-line graph that shows the total weekly fares for each city type. Finally, you’ll submit a written report that summarizes how the data differs by city type and how those differences can be used by decision-makers at PyBer. 
2. Requirements 
  * Create a ride-shareing summary DataFrame by city type. 
  * Create a multiple-line chart of total fares for each type 
  
## Analysis 

1. Deliverable 1: Ride-sharing summary DataFrame sorted by city type 
  * Merge two DataFrames from csv files 
  * Use the groupby() function to create a Series of data that has the type of city as the index, then apply the count() method on merged dataframe to the "ride_id" column to get the total rides for each city type. 
    Total rides by city type ![image](https://user-images.githubusercontent.com/82353749/118192343-fef85d00-b413-11eb-8cf8-911ff8036f3b.png)
  * Use the groupby() function to create a Series of data that has the type of city as the index, then apply the sum() method to the "driver_count" column.
    Total drivers by city type![image](https://user-images.githubusercontent.com/82353749/118193162-416e6980-b415-11eb-8942-4f3cfdc8a090.png)
  * Use the groupby() function to create a Series of data that has the type of city as the index, then apply the sum() method to the "fare" column.
    Total fares by city type![image](https://user-images.githubusercontent.com/82353749/118193464-bc378480-b415-11eb-87a3-b192758c0dfe.png)
  * Get the average fare per ride for each city type by dividing the total fares of each city type by the total rides of each city type; and get the average fare per driver for each city type by dividing the total fares of each city type by the total driver counts of each city type. 
    avg fare by ride/driver![image](https://user-images.githubusercontent.com/82353749/118194416-56e49300-b417-11eb-99c7-4dd08547992e.png)
  * Create a summary DataFrame from data retrieved from above. 
    Pyber_summary_df![image](https://user-images.githubusercontent.com/82353749/118194857-176a7680-b418-11eb-85db-7e69aa279eda.png)
  * Format pyber_summary_df 
    Formatted pyber_summary_df![image](https://user-images.githubusercontent.com/82353749/118195351-0ec67000-b419-11eb-9b5e-e3eaeea59ac1.png)
    
2. Deliverable 2: A multiple-line chart of total fares for each city type 
  * Using groupby() to create a new DataFrame showing the sum of the fares for each date where the indices are the city type and date.
    Total fares groupby city type and date![image](https://user-images.githubusercontent.com/82353749/118281454-38c07680-b49b-11eb-9360-c1532a707505.png)
  * After reset the index of the dataframe, use the pivot() function to convert the DataFrame from the previous step so that the index is the "date," each column is a city "type," and the values are the "fare." 
    Index as date![image](https://user-images.githubusercontent.com/82353749/118289833-bb4d3400-b4a3-11eb-96de-fe88585b6a5c.png)
  * Create a new DataFrame from the pivot table DataFrame using loc on the given dates, '2019-01-01':'2019-04-29'. 



