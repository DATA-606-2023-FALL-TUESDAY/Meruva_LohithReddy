# Capstone Proposal
 
## 1. Proposal Title: Electric Vehicle Classification

- **Author Name** - Lohith Reddy Meruva
- Prepared for UMBC Data Science Master Degree Capstone by Dr Chaojie (Jay) Wang
- <a href="https://www.linkedin.com/in/lohithreddy007/"><img align="left" src="https://img.shields.io/badge/-GitHub-CD5C5C?logo=github&style=flat" alt="icon | LinkedIn"/></a> 
  
- <a href="github.com/lo-hith"><img align="left" src="https://img.shields.io/badge/-LinkedIn-1E90FF?logo=linkedin&style=flat" alt="icon | GitHub"/></a>  
- **PowerPoint presentation file** - In Progress
- **YouTube video** - In Progress 
    
## 2. Background

 Because the EV market is expanding, it's critical for manufacturers, legislators, and consumers to understand the many types of EVs on the market. Knowing how many battery electric and plug-in hybrid vehicles are on the road at any one time is critical for successful infrastructure planning, regulation, and market segmentation. Through the construction of an accurate categorization model, this initiative aims to improve electric vehicle research, development, and decision-making.

 The purpose of this study is to learn more about the classification of EVs and to create a classification model that can correctly identify the type of EV, distinguishing between BEVs and PHEVs (Battery Electric Vehicles and Plug-in Hybrid Electric Vehicles).

**Research Questions:**
-Which characteristics of electric vehicles have the strongest associations with one another? The interdependencies and 
 connections between various aspects may be better understood.
- Analyzing the distribution of my target variable '**Electric Vehicle Type'** ?
- Geograhical analysis like ,How does the use of EVs vary from region to region, metro area to metro area, and state to 
  state? Is there a correlation between distance and the number of EVs on the road?
- What characteristics of a car determine whether or not it qualifies for the Clean Alternative Fuel car tax break?
- How does the electric utility provider affect the range of electric cars and whether or not they qualify for incentives?

## 3. Data 

Describe the datasets you are using to answer your research questions.

- **Data sources** - This dataset is collected by a Department of Licensing , which is published by data.wa.gov.
  - **Dataset Link:** https://catalog.data.gov/dataset/electric-vehicle-population-data 
- **Data size** - 35.3 MB
- **Data shape** -
  - Rows = 143596 
  - Columns =  17 
- **Time period** - 2023-08-14
- **Rows** - Electric Car Details
- **Data Dictionary**
-  VIN (1-10): Partial vehicle identification number consisting of the first 10 digits.
- What specific attributes within the Electric cars-] data have the highest correlation ?
- VIN (1-10): Partial vehicle identification number consisting of the first 10 digits.
- County: The county where the vehicle is registered.
- City: The city where the vehicle is registered.
- State: The state where the vehicle is registered.
- Postal Code: The postal code of the vehicle registration location
- Model Year: The year the vehicle was manufactured.
- Make: The manufacturer or brand of the vehicle.
- Model: The specific model of the vehicle.
- Electric Vehicle Type: Indicates whether the vehicle is a Battery Electric Vehicle (BEV) or a Plug-in Hybrid Electric -Vehicle (PHEV)
- lean Alternative Fuel Vehicle (CAFV) Eligibility: Indicates if the vehicle is eligible for Clean Alternative Fuel Vehicle benefits.
- Electric Range: The range of the vehicle on a full electric charge.
- Base MSRP: The manufacturer's suggested retail price for the vehicle.
- Legislative District: The legislative district associated with the vehicle registration location.
- DOL Vehicle ID: Unique identifier assigned by the Washington State Department of Licensing.
- Vehicle Location: The precise location of the vehicle.
- Electric Utility: The electric utility company associated with the vehicle.
- 2020 Census Tract: The census tract where the vehicle is registered.

  Which variables/columns may be selected as features/predictors for your ML models?

  My Target variable is **Electric Vehicle Type'** and my  feature variables be like 'Make','Model','Electric Range','Clean 
  Alternative Fuel Vehicle (CAFV) Eligibility','Legislative District','Electric Utility','Location' and after drawing a 
  heat map we can clearly make the decision which are highly correlated with my target variable 'Electric vehicle Type'. 
  
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
