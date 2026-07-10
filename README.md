# Siyang's data analysis and data science portfolios

Welcome to my github page! My name is Siyang Cai. I'm a reasearcher in Leicester University working in the area of data analysis and data sciecne of summary statistics from genome-wide association studies (GWAS). This is a list of my personal data analysis and data science projects as my portfolio.

## [Project 1: UK house price chatbot](https://siyangcai.github.io/UK-house-price-chatbot/)
This project is a local full-stack RAG application for UK housing market questions. I used FastAPI for the backend and React for the frontend. The system has two retrieval paths: structured retrieval from HM Land Registry Price Paid Data using DuckDB, and document retrieval from UK House Price Index reports using embeddings and FAISS.
For structured questions, the app calculates median sale prices, sales counts, date ranges, monthly trends, and area comparisons. For broader market or methodology questions, it retrieves relevant report passages and passes them to a local Ollama model. I also built query routing, geographic resolution, tests, a frontend chat interface, and a demo video.
- Built a full-stack RAG chatbot using FastAPI, React, Ollama, DuckDB, FAISS, and LangChain.
- Processed HM Land Registry Price Paid Data into Parquet and queried it with DuckDB for median prices, sales counts, trends, and area comparisons.
- Implemented document retrieval over UK House Price Index reports using embeddings and FAISS semantic search.
- Designed an LLM query-routing flow to classify questions into structured, document, hybrid, summary, trend, and comparison tasks.
- Built a geographic resolver to handle area names and area types such as city, district, county, and UK-level queries.
- Added a React chat interface with editable example prompts and connected it to the FastAPI backend.
- Wrote backend tests with pytest and documented the project with a GitHub README and demo video.

## [Project 2: Classification on poisonous and edible mushrooms](https://siyangcai.github.io/ML-mushroom-classification/)
This project aims to build machine learning models to help classify mushrooms between poisonous or eidble, which used a dataset contains hypothetical samples corresponding to 23 species of gilled mushrooms in the Agaricus and Lepiota Family Mushroom drawn from The Audubon Society Field Guide to North American Mushrooms. The main achievements are:
* comparing results from Logistic Regression, Support Vector Machine (SVM classifier) and a Voting classifer in scikit-learn,
* cross validation to avoid random effects on the whole pipeline of preprocessing and ML model,
* parameter tuning to find the best parameters with best accuracy,
* obtain best accuracy of 98.35% in identify poisonous mushrooms.

## [Project 3: House price prediction](https://siyangcai.github.io/House_price_prediction/)
This project aims to predict house prices by using machine learning models from a dataset that includes sale prices for King County in US in 2015. The main achievements in this project are:
* data cleaning to find some interesting information in the dataset and remove those that are unreasonable,
* feature engineering to create more feautres that better describe the sale prices,
* comparing results from Random Forest, Linear Regression, Lasso Regression and XGBoost, with cross validation.
* using parameter tuning if necessary,
* the best model is between Random Forest and XGBboost with a `R2` score as 0.99 

## [Project 4: Classification on images of car or trucks using CNN](https://siyangcai.github.io/car-or-truck/)
This is a classical deep learning project aiming to classify car and truck images using convolutional neural network. I have constructed a deep learning model with 3 CNN layers with data augments, followed by a training process with 80 epochs. I have not observed signs of over-fitting or under-fitting. An satisfying accuracy of 88.84% is then obtained.

## [Project 5: Cyclistic Case Study from Google Data Analytics Professional Course](https://siyangcai.github.io/Cyclistic/)
This is a capstone project from Google Data Analytics Professional Course, which aims to figure out user behaviour with/without membership using data from a bike-sharing company Cyclistic in 2021. The main achievements are:
* visualizations of the data in weekly and monthly form between casual and annual members,
* discovery of different using patterns between casual and annual members,
* Four possible solutions are designed to help increase membership subscriptions.
