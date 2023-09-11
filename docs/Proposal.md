# Capstone Proposal
 
## 1. Proposal Title: 

- **Author Name** - Lohith Reddy Meruva
- Prepared for UMBC Data Science Master Degree Capstone by Dr Chaojie (Jay) Wang
- <a href="https://www.linkedin.com/in/lohithreddy007/"><img align="left" src="https://img.shields.io/badge/-GitHub-CD5C5C?logo=github&style=flat" alt="icon | LinkedIn"/></a> 
  
- <a href="github.com/lo-hith"><img align="left" src="https://img.shields.io/badge/-LinkedIn-1E90FF?logo=linkedin&style=flat" alt="icon | GitHub"/></a>  
- **PowerPoint presentation file** - In Progress
- **YouTube video** - In Progress 
    
## 2. Background

Since the market for EVs is growing, it's important for manufacturers, legislators, and consumers to have a clear understanding of the many kinds of EVs available. For effective infrastructure planning, policymaking, and market segmentation, knowing how many battery electric cars and plug-in hybrid vehicles are on the road at any one time is crucial. This project intends to improve electric vehicle research, development, and decision-making via the creation of an accurate categorization model.

The goal of this research is to better understand how different types of electric vehicles are categorized and to develop a classification model that can accurately identify the type of electric vehicle, differentiating between Battery Electric Vehicles (BEV) and Plug-in Hybrid Electric Vehicles (PHEV).

**Research Questions:**
- What specific attributes within the Electric cars-] data have the highest correlation ?
- Which city is using highest electric vehicles.
- Analyzing feauter if Electrical Vehicle models
- How accurate are the machine learning models in predicting exploration of electric vehicles based on the  Department of Licensing  data?

## 3. Data 
-VIN (1-10): Partial vehicle identification number consisting of the first 10 digits.
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

Describe the datasets you are using to answer your research questions.

- **Data sources** - This dataset is collected by a Department of Licensing , which is published by data.wa.gov.
  - **Dataset Link:** https://catalog.data.gov/dataset/electric-vehicle-population-data 
- **Data size** - 35.3 MB
- **Data shape** -
  - Rows = 143596 
  - Columns =  17 
- **Time period** - 2023-08-14
- **Rows** - Car Details
- **Data Dictionary**
- 
    
  
- Which variables/columns may be selected as features/predictors for your ML models?

## 4. Exploratory Data Analysis (EDA)

- Perform data exploration using Jupyter Notebook
- Create visualizations (I recommend using **Plotly Express**)
- Find out if the data require cleansing:
  - Missing values?
  - Duplicate rows? 
- Find out if the data require splitting, merging, pivoting, melting, etc.
-  

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
