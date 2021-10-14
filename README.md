# CS573 Final Project Proposal (Final Version)

# Data
In this project, I would use "Crimes against to woman in India" dataset.  
https://gist.github.com/lzlazmSylas/6be318f1ef48498d10f831bbd78782f3   
This date set contains the crime cases information of different districts in each state in Inda from 2001 to 2014. I will visualize this data set in my project.    

**Attribute：**   

| Name | Type | Description |
| :--- | :----: | :---- |
| STATE | Categorical | state in india   |
| DISTRICT    | Categorical      | district in state       |  
| Year    | Ordinal     | Year     |  
| Rape    | Quantitative     | number of rape     |  
| Kidnapping and Abduction    | Quantitative      |  number of kindnapping and abduction     |   
| Dowry Deaths    | Quantitative      | number of dowry death     |   
| Assault on Women    | Quantitative      | number of assaulting     |   
| Insult to Modesty of Women    | Quantitative      | number of insulting case     |   
| Cruelty by Husband or His Relatives    | Quantitative      | number of cruelty by hubsband or victim's relatives    |   

 
# Questions and Tasks
- Which state have highest total number of specific crimes in each year. (bar chart)
- Which state have highest number of crimes for each type of crime. (pie chart)
- What kind of crime take the largest precentage among the all kind of crimes for each year. (pie chart)
- How does total number of crimes occured in each state compare to each other? The more intuitive version of crime cases! (map cahrt)

# Prototype
**The first prototype(basic bar chart)**  
This is the bar chart showing the total number of rape cases for each state in 2008. The X-axis represent the total number of given cases, the Y-axis represent each state in India.  
![image](https://github.com/lzlazmSylas/CS573-Final-Project-Proposal-Rough-Draft/blob/main/0001.png)
 
**The second prototype(Interactive bar chart)**  
Adding two drop down menu to the bar chart. One for filtering data by year that cases occored, another one is to filter the data by specific type crime case.  
All data are sorted in descending order so the first question will be solved in this interactive bar chart.   
![image](https://github.com/lzlazmSylas/CS573-Final-Project-Proposal-Rough-Draft/blob/main/0002.png)   
https://vizhub.com/lzlazmSylas/bc8f3f3d95fd46418a057950afec3480     

# Sketches
**Pie chart one**  
This pie chart will show the percentage of the total number of cases of each crime type in each year.  
There is one dropdown menu stick to this pie chart, it allows user to select the specific year then pie chart will be immediately rendered based on that.  
![image](https://github.com/lzlazmSylas/CS573-Final-Project-Proposal-Rough-Draft/blob/main/piechart01.png)  

**Pie chart two**  
# Schedule of Deliverables
This pie chart will show the percentage of the total number of cases with its associated state by the given crime type. In this pie chart, the number will be counted from 2001 to 2014.    
There is one dropdown menu stick to this pie chart, it allows user to select the specific year then pie chart will immediately rendered based on that. 
![image](https://github.com/lzlazmSylas/CS573-Final-Project-Proposal-Rough-Draft/blob/main/piechart02.png) 

**Map chart**  
This map chart will show the total number of crime cases in different state by the given year and crime type, so this chart will be link to the interative bar chart.   
They both share the two dropdown menu bound to barchart. When the element under the dropdown menu chaged, the map char will be rendered again.   
The state will be marked as one of the colors and the darker the color, the higher the crime rates.  
In this case I define the crime rate is equal to the number of selected type of crime for a state/ total number of crime for the given year.  
![image](https://github.com/lzlazmSylas/CS573-Final-Project-Proposal-Rough-Draft/blob/main/mapchart.png)  
# Schedule of Deliverables  
**Week 7**
- Finish the interative bar chart

**Week 8**  
- Finish the first pie chart  
 - Create an new pie chart
 - Add an interactive dropdown menu  

**Week 9**
- Finish the second pie chart  
 - Create an new pie chart
 - Add an interactive dropdown menu  

**Week 10**
- Create the map chart 
 - Make sure the state in dataset can match to the map chart


**Week 11**
- Link the map chart to the bar chart
 - Try to make then share both two dropdown menu
 
**Week 12**  
- Try to bound all chart into one html page
- Unit test

**Week 13**
- Unit test
- Submit the final version of priject  

# Possible Question
- The some name of state maynot match to the mapchart build in d3.  
