# CS573 Final Project Proposal (Final Version)

# Data
In this project, I would use "Crimes against to woman in India" dataset.  
https://gist.github.com/lzlazmSylas/c5d21ca1a87fefbe69f6b927a035db58
This data set contains the crime cases information of different districts in each state in Inda from 2001 to 2014. I will visualize this data set in my project.    
The other one is the data set contains population information of India:  
https://gist.github.com/lzlazmSylas/0e697ec5c8735d06eb660f0a81c61bee

# Project  
https://vizhub.com/lzlazmSylas/1505e03e7a4d4f4aa0f8b685a9da09ea?edit=files&file=index.js&mode=full
**Attribute：**   
First data set that describe the total criminal cases in India.  
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

The second data set contains population information of India.  
| STATE | Categorical | State in india   |   
| Year    | Quantitative  | population of each state fo specific year   |   

 
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
Adding two drop down menu to the bar chart. One for filtering data by year that cases occored, another one is to filter the data by specific type crimes.  
All data are sorted in descending order so the first question will be solved in this interactive bar chart.   
![image](https://github.com/lzlazmSylas/CS573-Final-Project-Proposal-Rough-Draft/blob/main/0002.png)   
https://vizhub.com/lzlazmSylas/bc8f3f3d95fd46418a057950afec3480     

# Sketches
**Pie chart one**  
This pie chart will show the percentage of the total number for different types of crimes in each year.  
There is one dropdown menu stick to this pie chart, it allows user to select the specific year then pie chart will be immediately rendered based on that.  
![image](https://github.com/lzlazmSylas/CS573-Final-Project-Proposal-Rough-Draft/blob/main/piechart01.png)  

**Pie chart two**  
# Schedule of Deliverables
This pie chart will show the percentage of the total number of cases with its associated state by the given criminal type. In this pie chart, the number will be counted from 2001 to 2014.    
There is one dropdown menu stick to this pie chart, it allows user to select the specific year then pie chart will immediately rendered based on that. 
![image](https://github.com/lzlazmSylas/CS573-Final-Project-Proposal-Rough-Draft/blob/main/piechart02.png) 

**Map chart**  
This map chart will show the total number of criminal cases in different state by the given year and criminal type, so this chart will be link to the interative bar chart.   
They both share the two dropdown menu bound to barchart. When the element under the dropdown menu chaged, the map char will be rendered again.   
The state will be marked as one of the colors and the darker the color, the higher the crime rates.  
In this case I define the crime rate is equal to the number of selected type of crime for a state/ total number of crime for the given year.  
![image](https://github.com/lzlazmSylas/CS573-Final-Project-Proposal-Rough-Draft/blob/main/mapchart.png)  

# Whats New?  
![image](https://github.com/lzlazmSylas/CS573-Final-Project-Proposal-Rough-Draft/blob/main/MapChartFinalVerson.png)
https://vizhub.com/lzlazmSylas/bc2000e9af9a4e139a9e2d322c3ccc63?edit=files  
For this two weeks, I built the india map chart by d3 and tried to combine the interactive bar chart with the map chart. I made the bar chart and map chart interat with each other  
Now it has following functions:  
1. It allow user the filter the data by year and crime type. The filtered date will be shown as the bar chart, the darker the color, the higher the crime number.  
2. When one rectangle in the bar chart is selected, it will be highlighted and to corressponding state in map chart will also highlighted.
3. When moving the mouse over the map chart and hover the mouse over the map chart, the map shows the specific crime information for the selected state, also the bar chart will  be highlighted.
# Whats New(11.15)?    
![image](https://github.com/lzlazmSylas/CS573-Final-Project-Proposal-Rough-Draft/blob/main/Not_Final_Version.png)
https://vizhub.com/lzlazmSylas/dc2ea5bbb67b4ba69fca3c8885a46e2d?edit=files&file=index.html&mode=full   
At the end of the week, I have created two donut charts which allow user who figure out the percentage of criminal cases for some state in India and the percentage of the specific criminal cases among total crimes each year.  
I corrected some spelling mistake in this dataset and make all state in upper case and now all data can be randered correctly.  

New functions:  
1. The first donut charts allow user to find the percentage of the specific crimes among total crimes each year.  
2. The second donut chart make people tell the percentage of the specific crimes in each state.

# Whats New(11.24)?   
1. This week I import a new dataset that describe the total population of each state in India from 2001 to 2014.  
2. I only have data about 2001 and 2011 census of India which accurate to the population of each state. Then I have to use another data set that describe the total population of India to estimite the state population from 2001 to 2014.
3. Then the criminal rate can be counted as #(number) of total cases / every 100,000 resident.  
 

# Whats New(11.30)?   
1. Reconstruct the code, make sure all important part locate in a JS file.
2. When the mouse hove on the bottom donut chart, the donut chart and map chart will be highlighted only when their selected criminal type matched. Thus, there are no highlighting bar chart confuse users. 

# Current Challange  
~~1. Now I want to knwo the crime rate of each state， I may need to import or join another date set that include the population of India from 2001 to 2014.~~  
~~2. There is a animation combination among the second donut chart, bar chart and map chart. It may confuse people when they move the cursor over the donut chart to find the   percentage of spcific crimes in one state and the bar chart will hightlight the number of criminal case, even thought the information they shown may not related.~~  

# Reference:    
1. World Population Prospects 2019 ： https://population.un.org/wpp/
2. Cencus 2001: https://www.census2011.co.in/states.php
3. https://en.wikipedia.org/wiki/List_of_states_in_India_by_past_population#By_past_population_(1947_to_2011)  

# Schedule of Deliverables  
**Week 7**  
- ~~Finish the interative bar chart~~  

**Week 8**    
- ~~Add an interactive dropdown menu~~  

**Week 9**  
- ~~Crete a map chart and make it interative~~  
- ~~Make the map chart and bar chart interact with each other~~  
- ~~Fix bug~~  

**Week 10**  
- ~~Create donuts charts~~  
- ~~Make sure the all information from dateset can be matched to all charts~~  


**Week 11**
- ~~Conquer the challenges found in week 10~~ 
- ~~Import new dataset and do some calculations~~  
 
**Week 12**  
- ~~Try to bound all chart into one html page~~  
- ~~Unit test~~ 

