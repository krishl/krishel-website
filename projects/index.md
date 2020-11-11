---
layout: page
title: Projects
permalink: /projects/
---

This is a list of the Data Science and Web Development projects I have worked on.

# Data Science
Each project name links to the respective Jupyter notebook. Datasets are available upon request.

### [Project 1 - Analyzing borrowers’ risk of defaulting](https://github.com/krishl/data-science-projects/blob/main/project-1/ds-project-1.ipynb)
#### Libraries used: Pandas, NLTK

This project is to prepare a report for a bank’s loan division. Here we investigate if a customer’s marital status and number of children has an impact on whether they will default on a loan. The bank already has some data on customers’ credit worthiness.

The report will be considered when building a credit score of a potential customer. Credit scoring is used to evaluate the ability of a potential borrower to repay their loan.

---

### [Project 2 - Research on apartment sales ads](https://github.com/krishl/data-science-projects/blob/main/project-2/ds-project-2.ipynb)
#### Libraries used: Pandas

Here we are using the data from a real estate agency. It is an archive of sales ads for realty in St. Petersburg, Russia, and the surrounding areas collected over the past few years. We will use this data to determine the market value of real estate properties. The task is to define the parameters. This will make it possible to build an automated system that is capable of detecting anomalies and fraudulent activity.

There are two different types of data available for every apartment for sale. The first type is a user’s input. The second type is received automatically based upon the map data. For example, the distance from the downtown area, airport, the nearest park or body of water.

---

### [Project 3 - Analyzing profiltability of mobile prepaid plans](https://github.com/krishl/data-science-projects/blob/main/project-3/ds-project-3.ipynb)
#### Libraries used: Pandas, Numpy, Scipy

Two prepaid plans offered by a state mobile operator will be analyzed to determine which of the two plans is more profitable. The results will be based on the behavior data of 500 clients.

---

### [Project 4 - Analyzing success of games](https://github.com/krishl/data-science-projects/blob/main/project-4/ds-project-4.ipynb)
#### Libraries used: Pandas, SciPy

Historical game data containing user reviews, genres, platforms, and sales will be analyzed to identify patterns that determine whether a game will succeed in 2017 or not.

---

### [Project 5 - Analyzing ride-sharing patterns](https://github.com/krishl/data-science-projects/blob/main/project-5/ds-project-5.ipynb)
#### Libraries used: Pandas, SciPy

Ride-sharing data on multiple ride-sharing companies will be analyzed to find patterns, understand passenger preferences, and gain insight into the impact of external factors on rides.

---

### [Project 6 - Classifying data plans](https://github.com/krishl/data-science-projects/blob/main/project-6/ds-project-6.ipynb)
#### Libraries used: Pandas, Sklearn

Different models are investigated in order to recommend the correct phone plan based on subscriber behavior with the highest possible accuracy.

---

### [Project 7 - Predicting customer behavior](https://github.com/krishl/data-science-projects/blob/main/project-7/ds-project-7.ipynb)
#### Libraries used: Pandas, Sklearn

Data on clients’ past behavior and termination of contracts with a bank will be used to predict is a customer will leave the bank soon. A model with the maximum possible F1 score will be built.

---

### [Project 8 - Finding the best place for a new oil well](https://github.com/krishl/data-science-projects/blob/main/project-8/ds-project-8.ipynb)
#### Libraries used: Pandas, Numpy, Sklearn

Data on oil samples from three regions will be used to create a model that will help pick the region with the highest profit margin. The Bootstrapping technique will be used to analyze potential profit and risks.

Conditions:
- Only linear regression is suitable for model training (the rest are not sufficiently predictable).
- When exploring the region, a study of 500 points is carried with picking the best 200 points for the profit calculation.
- The budget for development of 200 oil wells is 100 USD million.
- One barrel of raw materials brings 4.5 USD of revenue The revenue from one unit of product is 4,500 dollars (volume of reserves is in thousand barrels).
- After the risk evaluation, only the regions with the risk of losses lower than 2.5% will be kept. From the ones that fit the criteria, the region with the highest average profit should be selected.


---

### [Project 9 - Predicting the amount of gold recovered from gold ore](https://github.com/krishl/data-science-projects/blob/main/project-9/ds-project-9.ipynb)
#### Libraries used: Pandas, Numpy, Scipy

Data is provided on gold ore extraction and purification. A machine learning model will be built to help optimize the production and eliminate unprofitable parameters.

---

### [Project 10 - Creating a data transforming algorithm](https://github.com/krishl/data-science-projects/blob/main/project-10/ds-project-10.ipynb)
#### Libraries used: Pandas, NumPy, Sklearn

The Sure Tomorrow insurance company wants to protect its clients' data. The task is to develop a data transforming algorithm that would make it hard to recover personal information from the transformed data.

The data will be protected in such a way that the quality of machine learning models do not suffer.

---

### [Project 11 - Building a model to determine used car values](https://github.com/krishl/data-science-projects/blob/main/project-11/ds-project-11.ipynb)
#### Libraries used: Pandas, LightGBM, Sklearn, CatBoost

Rusty Bargain used car sales service is developing an app to attract new customers. In that app, users can quickly find out the market value of your car. We have access to historical data: technical specifications, trim versions, and prices. We will build the model to determine the value.

Rusty Bargain is interested in:

- the quality of the prediction
- the speed of the prediction;
- the time required for training

---

### [Project 12 - Predicting the number of taxi orders for the next hour](https://github.com/krishl/data-science-projects/blob/main/project-12/ds-project-12.ipynb)
#### Libraries used: Pandas, LightGBM, Statsmodels, Matplotlib, Sklearn, Catboost

Sweet Lift Taxi company has collected historical data on taxi orders at airports. To attract more drivers during peak hours, we need to predict the amount of taxi orders for the next hour. We will build a model for such a prediction. The RMSE metric on the test set should not be more than 48.

---

### [Project 13 - Detecting negative reviews](https://github.com/krishl/data-science-projects/blob/main/project-13/ds-project-13.ipynb)
#### Libraries used: Pandas, NumPy, Math, Matplotlib, Seaborn, Re, Tqdm, NLTK, spaCy, LightGBM, Torch, Transformers

The Film Junky Union, a new edgy community for classic movie enthusiasts, is developing a system for filtering and categorizing movie reviews. The goal is to train a model to automatically detect negative reviews. We'll be using a dataset of IMBD movie reviews with polarity labelling to build a model for classifying positive and negative reviews. The goal is to have an F1 score of at least 0.85.

---

### [Project 14 - Predicting the approximate age of a person from photographs](https://github.com/krishl/data-science-projects/blob/main/project-14/ds-project-14.ipynb)
#### Libraries used: Pandas, Tensorflow, Matplotlib

Supermarket chain Good Seed is introducing a computer vision system for processing customer photos. Photofixation in the checkout area will help determine the age of customers in order to:

- Analyze purchases and offer products that may interest buyers in particular age groups
- Monitor clerks selling alcohol

Here we will build a model that will determine the approximate age of a person from a photograph. To help, we'll have a set of photographs of people with their ages indicated.

---

# Web Development

![Luminance](https://angel.co/cdn-cgi/image/width=207,height=132,format=auto,fit=scale-down/https://s3.amazonaws.com/poly-screenshots.angel.co/Project/11/610203/d5d086357fee2074c4ac3fce565d2d6a-original.png)

  ***Luminance** - Compare ingredients between skincare products*

Everybody is different in their own way, and this statement does not exclude our skin's reactions to skincare ingredients. This tool compares ingredients between skincare products to aid in identifying beneficial and/or detrimental ingredients.

+ Constructed **single-page application** using **React** and **Redux** to create a dynamic user experience  
+ Created **backend API** with **Ruby on Rails** and **PostgreSQL**  
+ Used **Jbuilder** to generate **JSON** objects  
+ Utilized **Aphrodite-JSS** to style pages with custom **CSS** Stylesheets  
 
 View my blog post about Luminance at  [https://krishl.github.io/compare_skincare/](https://krishl.github.io/compare_skincare/)

[GitHub](https://github.com/krishl/sk-client) | [Demo](https://youtu.be/OR25Jn-b5Hs) | [Live](https://whispering-reaches-27170.herokuapp.com/)

---

![PlanEat](https://angel.co/cdn-cgi/image/width=207,height=132,format=auto,fit=scale-down/https://s3.amazonaws.com/poly-screenshots.angel.co/Project/67/610215/74fc6abf7dffc10a62a3ba8f336657ec-original.png)

  ***PlanEat** - Record and browse future dining plans by restaurant and by menu item*

This Rails app was created for those who often discover new restaurants and foods to try and need a place to record these new discoveries for later.
 
+ Constructed **RESTful API** with **Ruby on Rails** framework
+ Implemented **OAuth authentication** with **GitHub** using **OmniAuth**
+ Used **ActiveModel Serializers** to generate custom **JSON** for **Javascript** and **jQuery** features
+ Designed the **database schema** and configured **ActiveRecord** associations

View my blog posts about PlanEat at [https://krishl.github.io/restaurant_planner/](https://krishl.github.io/restaurant_planner/) and [https://krishl.github.io/jquery_restaurant_planner/](https://krishl.github.io/jquery_restaurant_planner/)

[GitHub](https://github.com/krishl/restaurant-planner) | [Demo](https://youtu.be/dHIpagwbFAg)

---

![BrewTeaful](https://angel.co/cdn-cgi/image/width=207,height=132,format=auto,fit=scale-down/https://s3.amazonaws.com/poly-screenshots.angel.co/Project/29/610217/a0125687ca29ebfae19d61c047123cbf-original.png)

  ***BrewTeaful** - Track the teas you own and discover new ones*

Brewteaful is a tool designed for tea lovers who would like an easier way to keep track of all the different kinds of tea that they own. Use this tool to record important tea brewing information such as: brewing time, brewing temperature, purchase date, and measurements. Also, discover new teas by viewing the latest submissions of fellow users.
 
+ Built **content management system** using **Sinatra** and the **MVC pattern**
+ Incorporated **ActiveRecord** to manage **SQLite database**
+ Utilized **BCrypt** to secure **user authentication** system
+ Designed **front-end** with custom **CSS**

View my blog post about BrewTeaful at [https://krishl.github.io/tea_tracker/](https://krishl.github.io/tea_tracker/)

[GitHub](https://github.com/krishl/tea-tracker) | [Demo](https://youtu.be/ePRSymu5SNw) | [Live](https://calm-stream-16313.herokuapp.com/)

---

![Potatotainment](https://angel.co/cdn-cgi/image/width=207,height=132,format=auto,fit=scale-down/https://s3.amazonaws.com/poly-screenshots.angel.co/Project/b5/610218/ab63c0e64da5bc0d1301e8e15f4832aa-original.png)

  ***Potatotainment** - Displays currently trending entertainment based on real-time check-in data*

This Ruby gem lists all currently trending shows and movies along with their respective details based on real-time check-in data from Trakt.tv for those who are having a hard time deciding what to watch.
 
+ Created **Ruby gem** aligned with **object oriented design principles**
+ **Scraped** a website using **Nokogiri** to obtain up-to-date **data**

View my blog post about Potatotainment at [https://krishl.github.io/trending_entertainment_cli_gem/](https://krishl.github.io/trending_entertainment_cli_gem/)

[GitHub](https://github.com/krishl/trending-entertainment-cli-app) | [Demo](https://youtu.be/WzMI70dfPSE) | [Live](https://rubygems.org/gems/trending_entertainment_cli_app)
