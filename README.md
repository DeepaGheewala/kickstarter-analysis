# kickstarter-analysis

## Overview of Project
 **Theater Data Analysis** - Here we need to find out how different campaign faired in relation to their launch dates and their funding goals

### Purpose
   * Find how Plays are performing during different months and based on different Goals

## Analysis and Challenges
 **Analysis**
   * The data provided is for fund raising events in different sectors (categories). The data provides the success rate and failure rate in achieving the goal 
   * For displaying monthly progress of Play, first it was required to covert the Unix format date to appropriate readable format.
   * For applying filter on Categories and subcategories it was good to have seperate column. 
   * Project File can be accessed here [Fund Raising Events Data - Kickstarter-analysis.xlxs](https://github.com/DeepaGheewala/kickstarter-analysis/blob/7c005a538be80fbf2800793a86f36a748c60ef65/Kickstarter_Challenge.xlsx)
 **Challenges**

   * Made the date conversion using this formaula '(((<columnName>/60)/60)/24)+DATE(1970,1,1)'
   * Extracted Categories using 'LEFT(<ColumnName>,SEARCH("/",<ColumnName>)-1)'
   * Extracted SubCategories using "RIGHT(<ColumnName>,LEN(<ColumnName>) - SEARCH("/",<ColumnName>))"

### Analysis of Outcomes Based on Launch Date

   - In the month on May there were more Successful campaign Plays
   - In Dec the success rate is almost similar to failure rate of campaign plays
   - A failed Play trend has less variations in diferent months
   - A successful Play trend has much variations in different months. 
   - Here is [Theater Outcomes vs Launch Date Chart](https://github.com/DeepaGheewala/kickstarter-analysis/blob/49cf0398d630d3f4499e05b91a794a95c4ce6040/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
   - The Percentage of Successful and Failure trend works opposite to each other for each goal ie. when Successful rates are higher, failure rates are lower.
   - The trend line have been very varying over different goals.
   - There is more success when the amount of fund raising is less.
   - Here is [Outcomes vs Goals Chart](https://github.com/DeepaGheewala/kickstarter-analysis/blob/49cf0398d630d3f4499e05b91a794a95c4ce6040/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
   - Understanding Github and writing analysis
      
  
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  - In the month on May there were more Successful Plays
  - In Dec the success rate is almost similar to failure rate of plays

- What can you conclude about the Outcomes based on Goals?
  - The Percentage of Successful and Failure trend works opposite to each other for each goal ie. when Successful rates are higher, failure rates are lower.

- What are some limitations of this dataset?
  - Cannot predict from date if the fund raising amount is more what would be the success or failure rate due to the variations.

- What are some other possible tables and/or graphs that we could create?
  - The a graph of amount pledge every month for the Plays
  - Country wise successful , failed and cancelled events
  - Categorywise donation collected
  
