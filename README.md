# Project-One

EV Sales vs. EV Chargers

Hypothesis: The number of EV’s sold will have an effect on the number of EV chargers built.

Null Hypothesis: The number of EV’s sold will not have an effect on the number of EV chargers built.

To start this analysis, I gathered data from iea.org, International Energy Agency. The dataset was in CSV format. The data was read in and turned into various Python Pandas Dataframes. Once separated I looked at the number of EV’s sold per year in China, Europe, USA, and the whole world. Next, I looked at the number of EV chargers built per year in the same locations. As can be seen by the graphs in the presentation China is clearly in front of the pack with EV sales and EV charging stations. Last I used linear regression to analyze EV’s sold vs. Number of EV Chargers. The regression model shows a strong positive correlation between the data sets. With a very high R^2 value of 0.9854 and a very low P value of 2.18e-12 the hypothesis has been confirmed and the null hypothesis has been rejected.


EV GLOBAL SALES

From the graph "Yearly Vehicle Sales by Country and Type (2000-2023)," we can derive several conclusions regarding EV (Electric Vehicle) sales in the specified regions:

United States:
EV Sales have seen a gradual increase over the years but are still significantly lower compared to non-EV sales.
The gap between EV and non-EV sales remains substantial, indicating slower adoption of EVs.

China:
China leads in EV sales among the regions compared.
EV sales have shown a steady upward trend, suggesting strong adoption and investment in EV technology.
Despite this growth, non-EV sales still dominate the overall market, but the gap is closing faster compared to other regions.

Rest of the World:
EV sales in this category are almost negligible, indicating either a lack of adoption or insufficient reporting of EV sales data.
Non-EV sales continue to dominate, with minimal representation of EVs.

Europe:
Europe has shown a consistent and moderate level of EV sales growth.
EV adoption is higher than in the United States but lower than in China.
Similar to China, while non-EV sales still lead, the increase in EV sales reflects a positive trend towards EV adoption.

Overall Inference:
China is the front-runner in EV sales, showcasing a significant move towards electric vehicles, likely driven by governmental policies and incentives.
Europe follows with a steady increase in EV adoption, reflecting environmental policies and growing consumer interest in sustainable transportation.
The United States shows growth in EV sales but at a slower pace, indicating potential barriers such as infrastructure, market readiness, or consumer preferences.
The Rest of the World category indicates minimal EV presence, pointing to possible challenges in EV adoption or data availability.
These conclusions highlight the varying levels of EV adoption across different regions, with China leading the way, followed by Europe, the United States, and the Rest of the World. The overall trend suggests a global shift towards EVs, but the pace and extent of adoption vary significantly.

How EVs Impact Emissions
This analysis focuses on CO2 Emissions by Country and how they relate to EV sales growth and incentives granted over the past decade. China seems to lead in EV sales against US and Europe almost every year since 2016. However, overall, their emissions only seem to be rising. The US and Europe have increasing sales, but their emissions have not dropped as sharply as the EV sales have gone up. You would think that EV adoption should reduce CO2 emissions, but they are greatly influenced by other factors (electricity grid sources, total vehicles on the road, and other industrial emissions).
When you look at the average of emissions by country over the past decade, China has the lowest average, even though they lead in sales. China had one drop in emissions between 2021 and 2022, which was when they had the most EV incentives in place. Europe also saw a decline in emissions between 2020-2023, which is when they had the most incentives in place. The US has the least amount of incentive policies by a significant amount, and we also have the highest average number of emissions by a significant amount. This shows that government policies can play a crucial role in how EVs impact total emissions. 

EV Polices vs. EV Sales - Jenn

Hypothesis: As more EV-friendly policies are announced, the number of EVs sold will increase.
Null Hypothesis: EV-friendly policies have no impact on the number of EVs sold.

Data sources: 
https://www.iea.org/data-and-statistics/data-tools/global-ev-policy-explorer (PDF)
https://www.iea.org/data-and-statistics/data-tools/global-ev-data-explorer (CSV)

Data preparation: Using similar methods as Justin for the EV Sales dataset above, I filtered and grouped the data to look at EV sales quantities for the following regions: USA, Europe, China, Rest of the World. Using Python, I charted each region's sales quantities over time, after removing projected data (anything related to 2025 and beyond). For the Policy Explorer dataset, I downloaded the PDF and converted it to CSV. Through a combination of Excel and Python, I calculated a record count for each country/region described above and created a bar chart showing the number of policies announced by region by year. Finally, I ran a pearsonr analysis to determine the correlation coefficient and p-value between the quantity of policies and the quantity of EV sales. 

Result: There is an overall positive correlation coefficient = 0.61 and a p-value =  5.88e-7 or 0.000000588. This positive r and low p-value indicate the two variables are positively correlated and we cannot reject the null hypothesis. It is not an especially strong correlation, however (only .6 compared to a value of 1, which would indicate perfect correlation). This is evidenced by the fact that new policies declined globally between 2022 and 2023, yet quantity of sales continued to go up. 



