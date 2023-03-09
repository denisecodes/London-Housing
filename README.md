# London Housing Dashboard

## Introduction

The idea of this project came from after I came across a Los Angeles Rental Pricing Dashboard made by Diane, you can find it <a href="https://www.mavenanalytics.io/project/472">here</a>. I moved to London in the summer of 2021 and have aspirations to settle down in the city and buy a property here in the future. So I decided to do this project to help myself, my friends and anyone else interested to buy a property in London in the near future.

<b>The aim of this project is to see analyze the following:</b>
<ul>
  <li>Relationship between Average Housing Price and Houses Sold from 1999 to 2020</li>
  <li>The Median Salary and Average Housing Price by Borough from 1999 to 2020</li>
  <li>Average Housing Price change from 1999 to 2020</li>
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

<img width="700" alt="Screen Shot 2023-03-09 at 22 13 33" src="https://user-images.githubusercontent.com/119052310/224172271-01de75d4-8c22-4cb1-9bb1-f9bd0eadb9b6.png">

I decided to differentate the average housing prices by using a colour gradient to higlight the most expensive boroughs in a bright, alarming red with the least expensive ones in an inviting green tone. I also thought adding the median salary of each borough in the tiptool would add more context, and see if there's any relationship between the median salary and average housing price of each London Borough.

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

<img width="313" alt="Screen Shot 2023-03-09 at 23 01 38" src="https://user-images.githubusercontent.com/119052310/224179748-7dbdef48-bcd0-46d6-847f-3e0045a51460.png">


## Key Findings

<b>Most expensive boroughs</b>
<ul>
  <li>Kensington and Chelseas</li>
  <li>City of Westminster</li>
  <li>Camden</li>
</ul>

<b>Least expensive boroughs</b>
<ul>
  <li>Barking and Dagenham</li>
  <li>Bexley</li>
  <li>Croydon</li>
</ul>

<b>Relationship between Average Housing Price and Houses Solds</b>


## Limitations 

## Further Analysis

## Conclusion


## Datasets used:

<ol>
<li><a href="https://www.kaggle.com/datasets/justinas/housing-in-london">London Housing Data 1999-2020</a></li>
<li><a href="https://data.london.gov.uk/dataset/statistical-gis-boundary-files-london">Statistical File of London Boroughs</a></li>
</ol>
