# Capstone Proposal
 
## 1. Proposal Title:"Flight Fare Prediction"

- **Author Name** - Lohith Reddy Meruva
- Prepared for UMBC Data Science Master Degree Capstone by Dr Chaojie (Jay) Wang
- <a href="https://www.linkedin.com/in/lohithreddy007/"><img align="left" src="https://img.shields.io/badge/-GitHub-CD5C5C?logo=github&style=flat" alt="icon | LinkedIn"/></a> 
  
- <a href="github.com/lo-hith"><img align="left" src="https://img.shields.io/badge/-LinkedIn-1E90FF?logo=linkedin&style=flat" alt="icon | GitHub"/></a>  
- **PowerPoint presentation file** - In Progress
- **YouTube video** - In Progress 
    
## 2. Background
 Since travel has become so important in our modern lives, finding cheap airline tickets is a top priority for many of us. The cost of a plane ticket might fluctuate depending on a number of variables such as the airline, the time of year, when the flight leaves, and what cabin class you're looking for. The ability to recognize the underlying trends in aircraft ticket price is very useful for travelers looking for economical and time-saving methods of planning their trips.

The goal of this research is to use data collected from the "Ease My Trip" website to better understand the complex dynamics at play in the airfare market. Not only do we want to be able to properly estimate flight costs, but we also want to be able to uncover important information that will aid passengers in their pursuit of affordable and convenient travel alternatives.

**Research Questions:**

-**Seasonal Trends:** Are there seasonal patterns in airport activity? If so, which months or times of year exhibit the highest levels of activity?

-**Airline Influence**: What airlines have the most effects on airport activity, and how do their numbers or the overall weight of landed cargo correlate to their presence?

-**Aircraft Types**: What sorts of aircraft, in terms of the number of landings and overall weight, contribute the most to airport activity?

-**Correlations**: What relationships exist between certain characteristics (such as landing count or total landed weight) and the desired variable (such as landing count or total landed weight)?

## 3. Data 

Describe the datasets you are using to answer your research questions.

- **Data sources** - This data set is taken from “Ease My Trip”
- **Dataset Link** - https://www.kaggle.com/datasets/jillanisofttech/flight-price-prediction-dataset
- **Data size** - 
- **Data shape** -
  - Rows = 10462
  - Columns =11
- **Time period** -January2019-Decemeber 2019
- **Rows** - 
- **Data Dictionary**
-  Airline:Type of Airline
-  Date_of_Journey
-  Source
-  Destination
-  Route
-  Dep_Time
-  Arrival_Time
-  Duration
-  Total_Stops
-  Additional_Info
-  Price

  Which variables/columns may be selected as features/predictors for your ML models?

  **Target Variable**: Price 
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
