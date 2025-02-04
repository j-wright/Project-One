# Project-One

EV Sales vs. EV Chargers
Hypothesis: The number of EV’s sold will have an effect on the number of EV chargers built.
Null Hypothesis: The number of EV’s sold will not have an effect on the number of EV chargers built.
To start this analysis, I gathered data from iea.org, International Energy Agency. The dataset was in CSV format. The data was read in and turned into various Python Pandas Dataframes. Once separated I looked at the number of EV’s sold per year in China, Europe, USA, and the whole world. Next, I looked the number of EV chargers built per year in the same locations. As can be seen by the graphs in the presentation China is clearly in front of the pack with EV’s sales and EV charging stations. Last I used linear regression to analyze EV’s sold vs. Number of EV Chargers. The regression model shows a strong positive correlation between the data sets. With a very high R^2 value of 0.9854 and a very low P value of 2.18e-12 the hypothesis has been confirmed and the null hypothesis has been rejected.
