The original dataframe from csv file:  
![image](https://github.com/user-attachments/assets/7ae97597-0de4-4beb-a12b-ed7d816f0f37)  
The best math schools taken by creating a dataframe of schools with columns school_name and average_math where average math is greater than 640 
and then sort DF by average_math with ascending=False so that the top marks are shown first
![image](https://github.com/user-attachments/assets/ea87c14f-a1e1-4d2f-8f10-679f07fb2f26)   
Top 10 schools is created similarly, except this is total_SAT column is created for the schools df and then truncated by .head(10)
![image](https://github.com/user-attachments/assets/21bab2b8-3456-468d-87bd-cd27b0909baf)   
Lastly, the borough with the largest standard deviation is shown along with its average_SAT(mean):
This is done by grouping the boroughs by total_SAT and invoking the .agg function on both mean and std rounded to two decimal points, then the max std of this 
dataframe is extracted then a new dataframe is created filtering where std is max_std
Then the count of boroughs is created on this df called num_schools
Finally, the dataframe's columns are renamed to average_SAT, std_SAT and num_schools  
![image](https://github.com/user-attachments/assets/80709cd9-0d02-4a80-bdfb-8f404b467fe2)



