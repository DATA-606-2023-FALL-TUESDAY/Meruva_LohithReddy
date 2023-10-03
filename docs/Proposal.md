# Capstone Proposal
 
## 1. Proposal Title:"Forecasting Airport Traffic: A Data-Driven Approach for the San Francisco International Airport"

- **Author Name** - Lohith Reddy Meruva
- Prepared for UMBC Data Science Master Degree Capstone by Dr Chaojie (Jay) Wang
- <a href="https://www.linkedin.com/in/lohithreddy007/"><img align="left" src="https://img.shields.io/badge/-GitHub-CD5C5C?logo=github&style=flat" alt="icon | LinkedIn"/></a> 
  
- <a href="github.com/lo-hith"><img align="left" src="https://img.shields.io/badge/-LinkedIn-1E90FF?logo=linkedin&style=flat" alt="icon | GitHub"/></a>  
- **PowerPoint presentation file** - In Progress
- **YouTube video** - In Progress 
    
## 2. Background

 Global logistics and transportation are greatly impacted by the aviation sector. For airport management, resource allocation, and capacity planning, it is essential to understand and plan for airport activities, such as the number of aircraft landings and the total weight of aircraft landed. Being a significant hub, San Francisco International Airport (SFO) generates a lot of operational data, including details on airlines, aircraft classes, and landing statistics. In order to estimate airport activity at SFO, this project will use data science and machine learning, offering insightful information to airport stakeholders.

In recent years, advances in data analytics and machine learning have made it possible to build accurate predictive models for various applications, including time series forecasting. In order to construct a prediction model that may predict future landing counts or total landed weight at SFO, this project will analyze historical data on airport landings and associated variables. It will also study temporal and location. patterns.


**Research Questions:**
-Seasonal Trends: Are there seasonal patterns in airport activity? If so, which months or times of year exhibit the highest levels of activity?

-Airline Influence: What airlines have the most effects on airport activity, and how do their numbers or the overall weight of landed cargo correlate to their presence?

-Aircraft Types: What sorts of aircraft, in terms of the number of landings and overall weight, contribute the most to airport activity?
-Correlations: What relationships exist between certain characteristics (such as landing count or total landed weight) and the desired variable (such as landing count or total landed weight)?

## 3. Data 

Describe the datasets you are using to answer your research questions.

- **Data sources** - https://www.flysfo.com/about/media/facts-statistics/air-traffic-statistics
- **Dataset Link** - https://data.sfgov.org/Transportation/Air-Traffic-Landings-Statistics/fpux-q53t
- **Data size** - 35.3 MB
- **Data shape** -
  - Rows = 30106
  - Columns =14
- **Time period** -2005-2023
- **Rows** - 
- **Data Dictionary**
-  Activity Period (timestamp)
-  Operating Airline
-  Operating Airline IATA Code.
-  Published Airline
-  Published Airline IATA Code
- 	GEO Summary.
-  GEO Region
-  Landing Aircraft Type
-  Aircraft Body Type
- 	Aircraft Manufacturer
- 	Aircraft Model
- 	Aircraft Version

  Which variables/columns may be selected as features/predictors for your ML models?

  Target Variable: Landing Count (Monthly landing counts at SFO)
## 4. Exploratory Data Analysis (EDA)

- Perform data exploration using Jupyter Notebook
- Create visualizations (I recommend using **Plotly Express**)
- Find out if the data require cleansing:
  - Missing values?
  - Duplicate rows? 
- Find out if the data require splitting, merging, pivoting, melting, etc.

## 5. Model Training 

- What models you will be using for predictive analytics?
- How will you train the models?
  - Train vs test split (80/20, 70/30, etc.)
  - Python packages to be used (scikit-learn, NLTK, spaCy, etc.)
  - The development environments (Juypter Notebook, Google CoLab, GitHub.)
- How will you measure and compare the performance of the models?

## 6. Application of the Trained Models

Develop a web app for people to interact with your trained models. Potential tools for web app development:

- **Streamlit** (recommended for its simplicity and ease to learn)
- Dash
- Flask

## 7. Conclusion

- Summarize your work and its potetial application
- Point out the limitations of your work
- Lessons learned 
- Talk about future research direction

## 8. References 

List articles, blogs, and websites that you have referenced or used in your project.
