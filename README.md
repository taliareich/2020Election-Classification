# U.S. Presidential Election 2020 - Predicting by County

# Business Problem
The Presidential election of 2020 was undoubtedly a major event in U.S. history. We all lived it; 2020 was a year of civil and political unrest, and the reality is that our country is still reeling. We witnessed firsthand how precarious democracy is, and the long-term impact of that election and this country's shifting political landscape is unknown. Political organizers rely heavily on insight regarding vote choice, since they know that big election years do not alone change politics, and much of the legwork happens at the individual and county level.
# Data
I used datasets containing information regarding [racial diversity](https://www.kaggle.com/mikejohnsonjr/us-counties-diversity-index), [election results](https://www.kaggle.com/unanimad/us-election-2020?select=president_county_candidate.csv), the CDC's [Social Vulnerability Index](https://www.atsdr.cdc.gov/placeandhealth/svi/data_documentation_download.html), and [unemployment rates](https://www.kaggle.com/carlosaguayo/2018-unemployment-rate-by-county). I’ve opted for the CDC’s Social Vulnerability Index dataset, which was used to help determine the toll COVID would take on individual counties, instead of COVID data since it is more generalizable to future elections. Since the data is broken up by county, and geographically, there are many more counties in typically red states, there is a class imbalance.
# Methods
Through various iterations of different classification models focusing on inference (logistic regression, random forest, etc.), normalizing features, and optimizing parameters, I was able to achieve my desired model and identify the most important indicators. 
# Results
My final logistic regression model had an f1-score of 73% and coefficient analysis showed, amongst other trends, that racial diversity is a good indicator for a win for Biden. 
# Further Analysis
More analysis is critical to getting a more nuanced view of what actually influences people to vote. Since this project focuses on binary outcome rather than voter turnout, a good next step would be to predict voter turnout numbers using similar data. 
# For More Information
Please see the jupyter notebook or the [presentation](https://docs.google.com/presentation/d/1PjT3O4Ms78N4XeKCgk1Cy33hIQaT3lvJbkLk30K5T5s/edit?usp=sharing).
## github repository

    ├── README.md                                         <- The top-level README for reviewers of this project
    ├── notebook.ipynb                                    <- Notebook
    ├── data                                    				  <- Folder containing data sources
