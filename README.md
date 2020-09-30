Life-Expectancy Analysis I analyzed the World Health Organization dataset of 22 different variables related to life expectancy over 193 countries for 15 years. A 2020 goal of mine is to fast 10% of the year. For me this became a 72 hour fast once a month. This was spurred on by Peter Attaia's research on extending life expectancy.

Naturally as I was looking for a project to show my data analytic capabilities the WhO's data set on longevity research was a gold mine. After looking at the columns and seeing there are 2938 entries with 20 quantitative and 2 qualitative features I wrote a for loop to find the null values in each column.

<img width="521" alt="Screen Shot 2020-09-30 at 11 56 24 AM" src="https://user-images.githubusercontent.com/68958681/94715982-cf2c9700-0313-11eb-8157-6313c64e8557.png">

For the variables 'Life_Expectancy' and 'Adult_Mortality' that have only 10 null values I filled these in with their mean. In hopes of getting a stronger line of best fit for my model I wrote functions to fill in the nulls with binned averages from a correlating variable.

<img width="642" alt="Screen Shot 2020-09-30 at 12 01 06 PM" src="https://user-images.githubusercontent.com/68958681/94716436-77daf680-0314-11eb-9436-ee4af3e4ff12.png">

This provided fun insights like seeing alcohol decrease after people received some schooling and then increase after a few more years of schooling. If we were to have filled in 'Alcohol' with its mean then this relationship would not have been shown.

BMI was a variable I trashed in the final analysis. The numbers didn't make sense. A morbidly obese BMI is over 40. The data had countries averaging over 80.

<img width="346" alt="Screen Shot 2020-09-30 at 12 13 43 PM" src="https://user-images.githubusercontent.com/68958681/94717631-3a776880-0316-11eb-89c2-566edc675fef.png">

I find it also worth mentioning that 'Alcohol' does have a positive correlation to Life Expectancy of 0.409865, but not a strong correlation. So double check those who are drinking for their health according to this study. 

During the process I also created a strong predictive model, but didn't find a great use case for it, so it was not added to my final analysis. 

Finally we have the analysis of looking at many different variables and then choosing those that correlated strongest with Life Expectancy for the final presentation. 

The two top indicators contributing to higher 'Life_Expectancy': 'Schooling' & 'Income_Comp_of_Resources. It is important to not mistake correlation for causation here. Though the more schooling a country receives it is most likely that the environment that allows increased schooling affects one's longevity rather than the time in front of a desk.

<img width="389" alt="Screen Shot 2020-09-30 at 12 19 43 PM" src="https://user-images.githubusercontent.com/68958681/94718223-110b0c80-0317-11eb-9b54-924ca64b5aa2.png">

The feature strongest correlated to a decrease in 'Life_Expectancy' is 'Adult_Mortality'. Adult Mortality is the rate of both sexes (probability of dying between 15 and 60 years per 1000 population). Since this doesn't lead to much explanation I saw what feature correlated strongest to Adult Mortality. The answer is HIV/AIDS.

To better undestand the effect of HIV/AIDS has on life Expectancy I plotted the 'Life_Expectancy' and 'HIV/AIDS' on the same world wide graph in Tableau. It is clear to see that the countries that have the highest ammounts of 'HIV/AIDS' also have the lowest 'Life_Expectancy'

<img width="945" alt="Screen Shot 2020-09-30 at 12 24 39 PM" src="https://user-images.githubusercontent.com/68958681/94718735-c3db6a80-0317-11eb-9040-c908d5fe596c.png">

The overall conclusion is the features that extend a countries life expectancy the most is a decrease of its population that has HIV/AIDS as well as how well the country can use its resources and the ability for the country to school its citizens.

Thank you for your attention. 
