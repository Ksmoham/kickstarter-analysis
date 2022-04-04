# Kickstarting with Excel

## Overview of Project

### Purpose
 
The purpose of this challenge is to organize a large crowdfunding dataset, make it user-friendly, and easier to analyze. The subcatagory I will be analyzing is the variables that contribute to the outcome of theater projects. This particular spreadsheet had 4116 rows and 14 columns. Sorting and filtering through the dataset by removing unnecessary information will allow it to be readable and convienient for predicting trends. Creating pivot graphs and charts with the filtered data will also make it easier to understand trends within the dataset.  

## Analysis and Challenges


### Analysis of Outcomes Based on Launch Date 

The goal of this analysis was to look at the outcome (succesful, failed, canceled) of theater productions based on which month it was launched. I filtered the data by spliting sub catogries from their parent catageories. This is so the we can only analyze plays and not all forms of theater. I also converted the unix timestaps using this formula "=(A1/86400)+DATE(1970,1,1)" in order for the date to appear in a mm/dd/yyyy.  pivot table and line graph were used to make the data easier to read and visualize. 
![Theater production outcomes based on launch date](https://user-images.githubusercontent.com/102334519/161501521-fea594f2-1392-4a9d-b70a-1c509829009d.PNG)

### Analysis of Outcomes Based on Goals

This data looked at the relationship between goal dollar-amount ranges and the outcome of plays. To sort through the large kickstarter dataset I used the COUNTIFS() function. This function allowed me to group multiple catagories together and filter through specific criterias. For example, "the number of successful plays which a budget goal of less than $1000" is a specific catagory, and without the COUNTIFS() would be difficult to filter through the entire dataset. I also used a pivot table and line graph to visualize the data. 

![Outcome based on goal](https://user-images.githubusercontent.com/102334519/161504340-43f30cfe-2b1e-4d72-8908-d0846ce55c47.PNG)

### Challenges and Difficulties Encountered

One of the difficulties I encountoured with this project was navigating the COUNTIFS() function on excel. Copying and pasting the formula from one cell and editing it to fit the criteria for another cell was tedious. However, after some researching I found that the MID function allowed me to extract text from inside a string. This made the process of grouping multiple catogories together easier.


## Results

What are two conclusions you can draw about the Outcomes based on Launch Date?

* one conclusion I can draw fromn the Outcome based on Launch date charts is that there is a high rate of succesful theater launches during the summer months. The highest success outcome was in May with a 66.87% success rate. Another conclusion I can draw is that compared the succussful productions, the failed productions showed a more consistent pattern.

What can you conclude about the Outcomes based on Goals?

* For the Outcomes based on Goals chart, it appears that most of the projects that were launched had a goal dollar amount of $10000 or less. 

What are some limitations of this dataset?

* One limitation of this dataset is that it lacks a genre catagory. Knowing which genres are more succesfull at which months and at which goal dollar amount may give her a better understanding of which campaigns and productions she should focus on. 

 What are some other possible tables and/or graphs that we could create?

* Comparing The US and GB on their campaigns and outcome could possibly help understand trends. A bar graph can be useful for this dataset. 



