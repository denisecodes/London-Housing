# London Housing Dashboard

## Introduction

The idea of this project came from after I came across a Los Angeles Rental Pricing Dashboard made by Diane, you can find it <a href="https://www.mavenanalytics.io/project/472">here</a>. I moved to London in the summer of 2021 and have aspirations to settle down in the city and buy a property here in the future. So I decided to do this project to help myself, my friends and anyone else interested to buy a property in London in the near future.

<b>The aim of this project is to see analyze the following:</b>
<ul>
  <li>Relationship between Average Housing Price and Houses Sold from 1995 to 2020</li>
  <li>The Median Salary and Average Housing Price by Borough from 1999 to 2020</li>
  <li>Average Housing Price change from 1995 to 2020</li>
  <li>Median Salary in London from 1999 to 2020</li>
</ul>

## Data Cleaning

<b>To set up the analysis and data visulization, I did the following to clean up the data:</b>
<ul>
  <li>Filtered out locations that were specific to London i.e. Scotland, Wales, England, United Kingdom etc.</li>
  <li>Inner joined London Housing monthly data, yearly data and London Borough spatial shape file</li>
  <li>Hide unnecessary columns for visualisation</li>
</ul>

## Data Visualizations

My goal was to complete the analysis I had set out to do to through data visualizations and combining them in to a Dashboard. I wanted my dashboard to have some interactive element to it and allow users to filter for data they are interested in.

### Filled Map: Median Salary and Average House Price by Borough

The first visualization I set out to do was a map that allows you to hover over and show you the average housing price for a specific London Borough as shown below. 

<img width="700" alt="Screen Shot 2023-03-10 at 13 47 08" src="https://user-images.githubusercontent.com/119052310/224332139-e247bc32-68e4-4ccc-aca3-7b3cb04384c1.png">

I decided to differentate the average housing prices by using a colour gradient to higlight the most expensive boroughs in a bright, alarming red with the least expensive ones in an inviting green tone. I also thought adding the median salary and total number of crimes of each borough in the tiptool would add more context, and see if there's any relationship between the median salary, number of crimes and average housing price of each London Borough.

### Numbers Table: London Overall

The next visualisation I made was a table to show key statistics that shows an overall picture of London. I decided the show the Median Salary, Average House Price and House Sold. 

<img width="525" alt="Screen Shot 2023-03-09 at 22 37 52" src="https://user-images.githubusercontent.com/119052310/224176202-0b3198b3-9d0e-4452-b16d-b136e4aeb9eb.png">

### Line Chart: Relationship between House Price and Houses Sold

Next, I wanted to see if there was any correlation between House Price and Houses Sold. To understand this well, I thought having two lines charts on the same graph would help me see the bigger picture as shown below. The green line refers to total number of houses sold whilst the yellow line refers to the average house price.

<img width="600" alt="Screen Shot 2023-03-09 at 22 40 30" src="https://user-images.githubusercontent.com/119052310/224176586-61fd4374-2deb-4fb2-9610-74eb48986ba1.png">

### Step Line Charts: Median Salary and Average Housing Price

Lastly, I wanted to understand the change and trend of Median Salary and Average Housing Price in London over the years, so I created the step line charts. The reason why I choose step line path instead of a usual line path is to to easily catch the big dips rather than just the overall trend of these parameters.

<img width="600" alt="Screen Shot 2023-03-09 at 22 47 32" src="https://user-images.githubusercontent.com/119052310/224177615-5e57e5bc-f9e3-40ad-aced-c7448d80f0d0.png">

<img width="600" alt="Screen Shot 2023-03-09 at 22 47 49" src="https://user-images.githubusercontent.com/119052310/224177663-7c21638d-8ff8-409f-a361-9a1c43fb1e2d.png">

## Filters

I created the following filters to allow users to drill down on specific data they are interested in:
<ul>
  <li>Housing Price Range</li>
  <li>Borough</li>
  <li>Year</li>
</ul>

<img width="319" alt="Screen Shot 2023-03-10 at 11 33 04" src="https://user-images.githubusercontent.com/119052310/224305720-330cce28-d655-4095-b68a-c8b95a93584d.png">

I decided to use the slider function for the Year filter for Map as it's really interesting to see the change in colour and truly reflects the housing price change over the last two decades in London. 

## Key Findings

<b>Most expensive boroughs over the years</b>
<ul>
  <li>Kensington and Chelseas</li>
  <li>City of Westminster</li>
  <li>Camden</li>
</ul>

<b>Least expensive boroughs over the years</b>
<ul>
  <li>Barking and Dagenham</li>
  <li>Bexley</li>
  <li>Croydon</li>
</ul>

These findings didn't come as a surprised to me as someone that has been living in London for 1.5 years with the knowledge I know about the city's rental prices, transport network, crime rate etc. What it really highlights is that there is a clear inbalance in the city's housing prices and the gap has further widened after 20 years. From this finding, I believe that the wealthier parts in the capital are still in the same areas whilst the poorer areas are continuing to stay poor. In fact, my opinion here is supported by the data provided by <a href="https://www.trustforlondon.org.uk/data/wealth-distribution/#:~:text=Wealth%20is%20very%20unequally%20distributed,of%20London's%20total%20net%20wealth.">Trust for London</a> from 2018 to 2020, where the organisation higlighted "<b>Wealth is very unequally distributed. In London, those in the top wealth decile (i.e. the 10% of people with the highest wealth) hold 44.3% of London’s total net wealth. Those in the bottom decile (the bottom 10%) hold none of London’s total net wealth.</b>" 

In conclusion, the finding here shows that wealth distribution in the capital has not changed much since 1999 with the wealth gap further widened and housing prices could be related to this. 

<b>Relationship between Average Housing Price and Houses Solds</b>

<img width="500" alt="Screen Shot 2023-03-09 at 22 40 30" src="https://user-images.githubusercontent.com/119052310/224176586-61fd4374-2deb-4fb2-9610-74eb48986ba1.png">

From this chart, we can see that the number of houses sold were on a steady rise between 1995 to 2002, before taking a small dip in between 2002 and 2005 before increasing again in 2006 until 2008. The dip after 2008 makes sense given the global financial crisis back then. Interestingly, we can see overall the average housing price has continued at a steady increase over the years, with a dip in 2008, which again does not come as a surprised given the economic climate. 

One of the biggest findings from this chart is when there was a big crash in the number of hosues sold from 2007 to 2008, indicating a massive drop in the housing marketing which correlates to the drop in the average housing price as the demand to buy a house decreased significantly. From my calculations using this dataset and visualization, the number of houses dropped by around 50% from 2007 and 2008. Since then, the number of houses sold has not gone back up to the numbers before 2008.

After the global financial crisis started to settle, the number of houses and the average housing price started to go back up in 2009. Interestingly, the number of houses sold started to drop after 2014 and has continued to decreased until 2020, whilst the average housing price has continued on a steady increase during this time. You can also see in 2016 when the two lines interesect, where the number of houses sold is now below the average housing price. The finding here correlates to me a lot and it shows that less and less people can afford to buy a house whilst the housing prices continues to increase. 

## Limitations 

The data cleaning process I did was not 100% thorough as there were duplicated rows of data during the process although I do believe the same number of records were duplicated. When I first inner joined the the files "<b>housing_in_london_yearly_variables.csv</b>" and the shape spatial file "<b>London_Ward_CityMerged.shp</b>", the number of rows increased significantly from 756 rows to 13293 rows. I believe the reason that Tableau did this was due to the necessity to keep all the data the the shape spatial file that would define the borders for the Lonodon Bouroughs as when I tried to clean up the data manually and make sure to keep the data at 756 rows, the London Boroughs did not show up properly. 

Base on the numbers reflected and my general knowledge, I believe the numbers do reflect the reality of the situation in London and for future analysis, it would be great to upgrade my current Tableau software with Tableau Prep or use other visualization softwares such as PowerBI to ensure throguh data cleaning. 

## Further Analysis

For future extension, I would like to look at the following for further analysis:
<ul>
  <li>Relationship between Weatlh Gap and House Prices, Houses Sold</li>
  <li>Relationship between People's Mobility and House Prices</li>
 </ul>

These first one would be interesting to look at as my hypothesis and findings indicate that there is likely a relationship Wealth Gap and Housing. 
Lastly, I believe the because of the increasing wealth gap in London, people's mobility and ability to move up in society could also be linked to the housing situation in London. 

## Conclusion and final thoughts

I really enjoyed doing for my first Data Visualization project. Most of the findings I found were not a surprise to me but seeing the change in the average housing prices over two decades in London was super interesting. What really striked out of all the findings was the number of houses sold since 2014 has continued in a steady decline. 

I believe this proejct helped to hone in my skills as a budding data analyst, practice the Tableau skills I have learnt from the courses I have taken and be able to apply it in a practical setting that can be applied to my career in Data Analytics. 

## Datasets used:

<ol>
<li><a href="https://www.kaggle.com/datasets/justinas/housing-in-london">London Housing Data 1995-2020</a></li>
<li><a href="https://data.london.gov.uk/dataset/statistical-gis-boundary-files-london">Statistical File of London Boroughs</a></li>
</ol>
