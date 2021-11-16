# School_District_Analysis
Module 4 - Jupyter Notebook Review

## Overview of Analysis
### Original Request
The original ask was to analyze school data from multiple schools within a district. Within this analysis is included:
- A Big Picture view of the disctrict's metrics
- A breakdown of these metrics into a per school basis
- Per school performance information
- Per grade performance information
**Note: any reference to "original" data in this summary is referencing the above request**

### Current Purpose of Analysis
The updated request for the data is related to academic dishonesty.  
Data from the freshman class at Thomas High School (THS) needs to be removed to confirm how much these altered grades affected the original analysis.  
By removing the fraudulent data and normalizing the remaining information, the school board can have a better understanding of the relationships between budget and grade outcomes. 
**Note: any reference to "adjusted" data in this summary is referencing the calculations once the count of THS 9th graders, and their scores, were removed from the calculations.

**Goals of the Module:** Using Python in Jupyter Notebook to navigate the basics of the Pandas library.
1. Create a development environment
2. Load and read raw data from CSV files
3. Review, clean, and confirm consistency of data
4. Merge datasets to allow for mathematical calculations
5. Visualize the data as part of a ReadMe on GitHub


## Results

#### District summary:
- Original District outcomes  ![image](https://user-images.githubusercontent.com/91762315/141832318-afdb85b3-5765-47d6-b960-079fbc87cbc5.png)
- Adjusted District outcomes  ![image](https://user-images.githubusercontent.com/91762315/141831840-b64fe796-e01e-4933-b1cf-fc27e2ae3d05.png)
- As you can see from the images, removing the 9th grade scores from THS did not have a large outcome on the district as a whole.
  - The difference between the original and adjusted averages for math and reading is neglible, <0.2%
  - The difference between the original and adjusted averages for percentage of students passing is slightly higer than the previous point, but still not to the point that it will make a large difference in reporting. 
  - The greatest difference is between the overall percentage of students passing, with a change of .3%

#### Per school summary:
- ![image](https://user-images.githubusercontent.com/91762315/141836274-9744eb4b-6b59-461d-b4ee-c174565baf33.png)
- ![image](https://user-images.githubusercontent.com/91762315/141836113-72508d0c-adc2-46b3-9227-0eec294326ce.png)
- This separate percentages of passing for Math and Reading as well as the overall passing percentage were adjusted by <.5%.
- The average scores were minimally affected, as they changed by less than one point each. Math decreased by .05 points, and Reading incerased by .05 points.

#### Adjusted scores affect on THS:
- The scores did not adjust THS's performance ranking compared to the other schools.
- THS was and remains the second highest ranked school, in overall percentage passing.
- Original listing  ![image](https://user-images.githubusercontent.com/91762315/141837602-118ceb95-2998-4891-b7b9-c845b24d9d51.png)
- Adjusted listing  ![image](https://user-images.githubusercontent.com/91762315/141837694-532c6f77-8e11-4a96-a786-a7dedaba8c17.png)

#### Breakdown of adjusted scores affect on THS:

#### Math and reading scores by grade
Removing the 9th grade scores shows that the scores are now listed as nan (Not a Number), indicating that it is no longer a part of the calculation. No other information was updated.

Original Reading Scores  
![image](https://user-images.githubusercontent.com/91762315/142035619-1634b227-87e5-4704-8742-7a2d8a353a29.png)

Adjusted Reading Scores  
![image](https://user-images.githubusercontent.com/91762315/142035501-9f83dce9-e090-4f66-9440-cfbd83336b08.png)


Original Math Scores  
![image](https://user-images.githubusercontent.com/91762315/142035436-23ec0f30-22fe-4dd4-bdc9-34b782dfcfaa.png)

Adjusted Math Scores  
![image](https://user-images.githubusercontent.com/91762315/142035301-88c1b075-03aa-4a2d-bd7a-875931b1ac9d.png)


#### Scores by school spending
Removing the 9th grade scores shows no change to the scores by school spending.

Original data left, Adjusted data right 
![image](https://user-images.githubusercontent.com/91762315/142036287-27f7ca75-fb00-473d-a8bd-f8401835d461.png)


#### Scores by school size
Removing the 9th grade scores shows one change to the medium (1500-2000) category.
The Average Math Score of this group went down by .1 points.

Original data left, Adjusted data right 
![image](https://user-images.githubusercontent.com/91762315/142037271-319ea6b7-5de7-434d-8f75-af62259edfad.png)

#### Scores by school type
Removing the 9th grade scores shows no change to the scores by school type.

Original data left, Adjusted data right 
![image](https://user-images.githubusercontent.com/91762315/142037644-5ad412f2-dafd-4311-a991-0398c24506b2.png)


## Summary
### Importance of balancing data
After the fraudulent scores were removed, adjustments were needed to ensure an accurate understanding of the outcomes.  By simply replacing the THS freshman scores with NaN, the calculations using total student count skewed the data.  Once the calculations were updated to remove the ninth-graders from the total student count, we identified the following points.

1. No changes occurred to the THS school ranking
2. No changes occurred to the scores by schoool type.
3. None of the percentages were changed more than .5% from the original data
4. None of the grades were changed more than .1 points
