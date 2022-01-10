# kickstarter-analysis

Performing analysis on kickstarter data to uncover trends

Overview of Project

  The purpose of this project was to learn how to manipulate various data types to produce analyses for the client's business use. We analyzed trends as well as learned how to convert data for better visualization. We also learned how to create tables and charts using pivot table functionality. From this project were able to identify successful, failed, and canceled artistic categories in various countries. We are also able to disaggregate the data by year, goal amount, and other variables. 
  
Analysis and Challenges

  For Deliverable 1, the first step required a date conversion from the UNIX time stamp that was provided in the data set. This conversion was success with the following formula: =(((J2/60)/60)/24)+DATE(1970,1,1). Once we populated with the converted date, we changed the data type from General to Short Date. This allowed us to visualize the data in way we can understand. From there, we extracted the year from that column using this forumula: =Year(). Next, we created a pivot table by filtering by parent category and years, outcome on the x-axis and months on the y-axis. Afterwards, we sorted the data and created a pivot chart that best displayed our data. 
    ![image](https://user-images.githubusercontent.com/96396696/148712019-8544766e-6f28-44ae-be93-94f2703e322c.png)
    ![image](https://user-images.githubusercontent.com/96396696/148712044-fdfac4fc-d85c-4d82-86e9-2b57a14beee9.png)
    
  For Deliverable 2, we populated our own table using the source data from the KickStarter tab. We used the =COUNTIF() formula to populate our successful, failed, and canceled plays based on goal range. Then we found the sum of each goal range as well as the percentage of successful, failed, and canceled plays. Next, we created a line chart with that data with the goal range on the x-axis and percentage of outcomes on the y-axis. I think the biggest challenge I faced was in Deliverable 2 due to simple errors like forgetting a comma or a dollar sign in the formula. 
    ![image](https://user-images.githubusercontent.com/96396696/148712088-5e267a7c-3905-4175-878c-7a1b68589f57.png)
    ![image](https://user-images.githubusercontent.com/96396696/148712095-f9c132d5-ddcd-4b15-9d43-7126b2db630c.png)

Results
  1. What are two conclusions you can draw about the Theater Outcomes by Launch Date?

     From this analysis we can conclude that in all the years, the month of May had the most successful outcomes for the parent cateogry 'theater'. After the month of May, the number of successful theater steadily declines. With respect to failed theater outcomes, the anaysis shows a rather steady data with the outcome range mainly between 31 and 52. Lastly, there were few canceled theater outcomes in all the years compared to successful and failed, and no data for the month of October.    
  2. What can you conclude about the Outcomes based on Goals?

     The number of successful outcomes for plays with a smaller goal is much higher than those with higher goals. This treand is also consistent with the number of failed outcomes. We do not have any data on number of canceled outcomes for plays. Interestingly, the percentage of of successful and failed outcomes with a goal of greater than $50,000 was higher than the goals between $10,000 and $49,999.   4. 
  3. What are some limitations of this dataset?
  
     A major limitation of the data was that it required a lot of data conversion for a single variable, and this may lead to errors in your data. For instance, the date launched column required a data conversion from UNIX and then againe to Short Date Change. One other limitation is that currency for the campaigns is different. For instance in Deliverable 2, we were looking at the goal range for all plays but there are different currencies included in this data therefore cannot be weighted the same. This is a major limitation in the analysis because $40,000 dollars in USD may be different than from another country. The data needs to be clearner for deliverable 2 by having a common unit of measurement for goal. I also think that another limitation of this data set is that there is no data dictionary. Without a data dictionary it is hard to truly understand the value of these variables and how they can be used to answer business questions.
  4. What are some other possible tables and/or graphs that we could create?
  
     Additionally, I think it would be helpfull to conduct an analysis on goal vs pledeged because this analysis may provide insight on the interest of the campaigns by donars. Perhaps campaigns that surpassed their goal by a certain margin can be priortized. Since we have the start and end dates of the campaigns we can further analyze the length of these campaigns and combine that with the suggested analysis mentioned to identify the most successful campaigns. We could also analyze the data by country, subcategory, and outcome to identify if there are differences is successful campaigns in different countries. 
