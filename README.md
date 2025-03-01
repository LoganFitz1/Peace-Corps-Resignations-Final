## Motivation for Analysis

The Peace Corps is a U.S. Government program that sends American volunteers all over the world to work on community-driven projects in education, health, agriculture, youth development, and more. The mission of the Peace Corps is to promote world peace and friendship by helping countries develop and build understanding between cultures. Volunteers typically commit two years of service and stay in their Country or region of assignment until service is complete.

Until recently, the Peace Corps kept their early-resignation data confidential to avoid potential backlash from reports of negative experiences. Thanks to the Data Liberation Project, this information is now publicly available and free to analyze. The Data Liberation Project is dedicated to acquiring, preserving, and sharing valuable public data that might otherwise remain inaccessible. By promoting transparency, the project empowers researchers, journalists, and the public to draw meaningful insights from newly available datasets. 

My motivation for analyzing this data comes from the unique opportunity to learn more about the experiences of past volunteers and to provide insight to future volunteers. With this information now publicly available, we can analyze patterns and trends of early volunteer departures and the primary reasons for leaving each Country. Insights from my analysis can help future volunteers make informed decisions when planning their service trips to curate a more positive and successful experience. Future analysis can build off my work by incorporating additional datasets to uncover deeper connections. For example, given data on which U.S. states volunteers come from, we could analyze how different backgrounds succeed or struggle in specific locations and provide tailored recommendations for volunteer placement.

Informative links:

[About the Peace Corps](https://www.peacecorps.gov/what-we-do/our-mission/)

[About the Data Liberation Project](https://www.data-liberation-project.org/about/)


## Data Overview
This dataset provides an overview of Peace Corps volunteers who resigned before the end of their natural service contract. Data is organized by service locations and the reasons for resignation, allowing volunteers to select up to two reasons for their early resignation. Each row represents an aggregate of the number of volunteers for each combination of reasons by Country. For example, if 5 Zimbabwe volunteers cited "mental health" and "amount of work," the count of that unique row would be 5. 

Data is available through July 31, 2023, but the start of the covered period is unclear. However, even with this limitation, the data reveals interesting trends for volunteer resignations and the potential conflicts that volunteers experience in various countries. In addition, I supplemented this analysis with a Peace Corps dataset (2007–2020), providing detailed insights into volunteer numbers and early resignations by Country and year. I cleaned this data by renaming variables for clarity, connecting sources through primary and foreign keys, using the coalesce function to manage null values by filling in the correct value or label, and creating measures and dimensions for coding efficiency.

Links to Data Sources:

[Data Liberation Project Data](https://www.data-liberation-project.org/datasets/peace-corps-resignations/)

[Early Resignation Data 2007-2020](https://www.peacecorps.gov/about-the-agency/policies-and-publications/reports-and-documents/?search_text=Early%20Termination%20Data%20by%20Country%20-%20Annual%20Method%20-%20FY%202007-2020%20%5BCSV%5D)

[Link to My Project Repository](https://github.com/LoganFitz1/Peace-Corps-Resignations-Final.git)


## Summary of Findings

My analysis of Peace Corps resignation data shows an average of 186 resignations per Country, with 2019 standing out as the peak year, totaling 4,128 early departures. The most common reason cited for leaving was "no reason listed" followed by family-related reasons, while Morocco recorded the highest number of resignations due to the "amount of work." Of all participating countries, only 14 had zero early terminations, highlighting the widespread nature of early departures. Africa led all regions in both the total number of volunteers and the highest number of resignations, demonstrating the unique challenges and demands of service in that continent. 

<img src="Total Volunteers by Region 2007 to 2020.png" alt=" Bar-chart: Total Volunteers by Region 2007 to 2020" width="50%">

The visual above displays the total number of Peace Corps volunteers from 2007 to 2020, segmented by region: IAP, EMA, and Africa. The chart highlights the steady increase in volunteers across each region category, with Africa consistently leading in volume total and a notable peak in 2019 for each region.

<img src="Scatter-plot.png" alt=" Scatter-plot: Total Volunteers by Country" width="50%">

The scatter-plot above is another unique visualization comparing the total number of volunteers across locations. Africa is a clear outlier, significantly surpassing all other locations.


<img src="Primary Reasons for Resignation by Country - Ecuador.png" alt=" Bar-chart: Primary Reasons for Resignation by Country - Ecuador" width="50%">

This visual provides an analysis of the most common reasons for quitting based on Country. This particular screenshot captures the Country of Ecuador; we can see that Ecuador, like many other Countries, received many resignations that listed no reason, followed by “unrealistic expectations” and “physical health”.

<img src="Safety-related Resignations.png" alt=" Bar-chart: Locations With Safety Concerns" width="50%">

Safety is a major concern when traveling internationally. The bar chart above shows Countries with the most number of safety-related volunteer resignations.

<img src="Increase Resignations in Africa.png" alt=" Line-chart: Increae in Resignations in Africa" width="50%">

The line chart above illustrates the trend in total Africa resignations from 2007 to 2020. The data reveals a steady rate of resignations until a sharp increase around 2015, almost doubling to  10,000 before tapering off slightly in 2019. This spike may indicate significant organizational or regional changes that impacted volunteer retention during this period.

<img src="Analysis of Work Related Resignations.png" alt=" Table view: Analysis of Work Related Resignations" width="50%">

This final screenshot captures an analysis highlighting countries with the most volunteer resignations due to "amount of work." Morocco leads with 26 resignations, followed by Benin, Albania/Montenegro, Rwanda, and Peru, each with 6. While this last graphic isn't the most visually appealing, this type of analysis can be valuable for service trip planning and demonstrates the analytical power of Malloy.


## Directions on How to Use GitHub Web Editor

Are you logged into github? Just press the period key right now. This will load the web editor. Then install the Malloy extension. Feel free to explore, experiment, and learn more about Peace Corps Volunteers!
See images below for direction references:
| **Step**   | **Image Preview** |
|--------|-----------|
| `Step 1 - Press allow` | <img src="step1.png" width="50%"> |
| `Step 2 - Click the Blocks, search for Malloy, install` | <img src="step2.png" width="50%"> |
| `Step 3 - Click Trust` | <img src="step3.png" width="50%"> |
| `Step 4 - Click a .malloynb file` | <img src="step4.png" width="50%"> |
| `Step 5 - Press Run` | <img src="step5.png" width="50%"> |
