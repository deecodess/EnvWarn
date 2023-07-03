![Logo](https://cdn.discordapp.com/attachments/806974540139200623/1125457812173094912/image-removebg-preview1.png)
<br/>
EnvWarn is a one-stop solution to all your climate action needs which predicts earthquakes, and flood events, and provides news summary, fundraising, and upcoming events alerts on natural disasters.

## Table of Contents
* [Background](#background)
* [Technologies](#technologies-used)
* [Glimpse](#glimpse)
* [Features](#features)
* [Flood Prediction Model](#the-flood-prediction-model)
* [Earthquake Prediction Model](#the-earthquake-prediction-model)
* [Hurricane Prediction Model](#the-hurricane-prediction-model)
* [Backend](#the-backend)
* [Frontend](#the-frontend)
* [Challenges I ran into](#challenges-i-ran-into)
* [Accomplishments](#accomplisments-that-i-am-proud-of)
* [What I learnt](#what-i-learned)
* [What's next?](#whats-next-for-envwarn)
* [Installation](#getting-started-with-the-project)


## Background
**Earthquakes:** 
India is located in a seismically active zone, with several tectonic plates converging in the region. As a result, the country experiences a significant number of earthquakes. On average, India witnesses around 5000 earthquakes annually, ranging from minor tremors to more significant seismic events. The most seismically active regions in India include the Himalayan belt, the northeastern states, and parts of Gujarat and Maharashtra. Here are few earthquake prone zones of India:
<br/>
![Earthquake-zones](https://media.discordapp.net/attachments/806974540139200623/1125455506245431346/image.png)

**Floods:** 
Floods are a recurrent natural disaster in India, affecting various regions due to heavy monsoon rains, cyclones, or dam failures. The country's vast river systems, such as the Ganges, Brahmaputra, and their tributaries, make it particularly vulnerable. Annually, India witnesses numerous floods, impacting millions of people and causing extensive damage to infrastructure, agriculture, and livelihoods. Here are few flood prone areas in India:
<br/>
![Flood-prone-areas](https://media.discordapp.net/attachments/806974540139200623/1125456054143176814/image.png)

**Hurricanes:** 
India's coastal areas, particularly along the Bay of Bengal and the Arabian Sea, are prone to cyclones or hurricanes. The cyclone season typically lasts from April to December, with the most intense activity occurring between October and December. Cyclones like Cyclone Biparjoy(2023), Cyclone Fani (2019) and Cyclone Amphan (2020) have caused significant devastation in recent years, affecting states like Odisha, West Bengal, Tamil Nadu, and Andhra Pradesh. Here are few Hurricane prone zones in India:
<br/>
![Hurrican-zones](https://media.discordapp.net/attachments/806974540139200623/1125456803203928215/image.png)

## Technologies used
With the implementation of principles of machine learning and deep learning, to predict the landslides and floods nearby, and statistical analysis of weather-map data, EnvWarn is an application fully powered by Flask at the backend, presented in web format. Though the code and structuring in the backend may look complex, the application is designed such that users won’t have trouble accessing the features. UI is as simple and intuitive as possible.

<p align="left">
    <a href="https://pytorch.org/" target="_blank" rel="noreferrer">
        <img src="https://img.shields.io/badge/pytorch-EE4C2C?style=for-the-badge&logo=PyTorch&logoColor=white" />
    </a>
    <a href="https://www.python.org" target="_blank" rel="noreferrer">
        <img src="https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue"
            alt="python" />
     <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer">
        <img src="https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="pandas"/>
    </a>
    <a href="https://www.figma.com/" target="_blank" rel="noreferrer">
        <img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white"  alt="figma"/>
    </a>  
     <a href="https://numpy.org/" target="_blank" rel="noreferrer">
        <img src="https://img.shields.io/badge/numpy-013243?style=for-the-badge&logo=numpy&logoColor=white"  alt="numpy"/>
    </a>
    <a href="https://matplotlib.org/" target="_blank" rel="noreferrer">
        <img src="https://img.shields.io/badge/matplotlib-EE4C2C?style=for-the-badge&logo=matPlotLib&logoColor=white"  alt="matplotlib"/>
    </a>
     <a href="https://colab.research.google.com/" target="_blank" rel="noreferrer">
        <img src="https://img.shields.io/badge/google%20colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white"  alt="google colab"/>
    </a>
    </p>

## Glimpse

![HomePage](https://cdn.discordapp.com/attachments/806974540139200623/1125452178237182043/image.png)
<h4 align="center">Home Page</h4>

![FloodPrediction](https://media.discordapp.net/attachments/806974540139200623/1125462061300863117/image.png?width=1025&height=450)
<h4 align="center">Flood Prediction</h4>

![EarthquakePrediction](https://media.discordapp.net/attachments/806974540139200623/1125461865586233374/image.png?width=1025&height=443)
<h4 align="center">Earthquake Prediction</h4>

![HurricanePrediction](https://cdn.discordapp.com/attachments/806974540139200623/1125461940953677994/image.png)
<h4 align="center">Hurricane Prediction</h4>


## Features
- Flood Prediction
- Earthquake Prediction
- Hurricane Prediction
- Providing Latest News about Natural Calamities
- Educating Users about safety during these disasters

## The Flood Prediction Model
**Dataset**
During August 2018, severe floods affected the south Indian state Kerala, due to unusually high rainfall during the monsoon season. It was the worst flood in Kerala in nearly a century. Over 483 people died, and 140 are missing. About a million people were evacuated. All 14 districts of the state were placed on red alert.
According to the Kerala government, one-sixth of the total population of Kerala had been directly affected by the floods and related incidents. The Indian government had declared it a Level 3 Calamity, or "calamity of a severe nature".
The dataset contains some data about 2018 Kerala flood casualties, warnings, district wise warnings, and rainfall.
[Dataset](https://sdma.kerala.gov.in/wp-content/uploads/2019/08/Memorandum2-Floods-2018.pdf)

**ML Models**
The prediction algorithms that I tested out were: 
- **KNN Classifier:**
KNN is well-suited for flood prediction due to its ability to capture non-linear relationships, adapt to changing patterns, and provide localized predictions based on nearest neighbors. Its simplicity, interpretability, robustness to outliers, and relatively fast training time make it a viable choice for flood prediction projects with complex and evolving data.
- **Logistic Regression:**
Logistic regression is used in flood prediction due to its ability to model the probability of a binary outcome, such as flood occurrence. It can handle both continuous and categorical variables, making it suitable for incorporating various factors like rainfall, water levels, and geographical features in predicting the likelihood of a flood.
- **Decision Tree Classification:**
The decision tree classifier is used in flood prediction due to its ability to handle complex decision-making processes and capture non-linear relationships between various factors, such as rainfall, water levels, and geographical features. It provides interpretability by visually representing the decision-making process and can handle both numerical and categorical data, making it suitable for analyzing diverse flood-related variables.
- **Random Forest Classification:**
The random forest classifier is used in flood prediction due to its ability to handle complex and high-dimensional data, capture non-linear relationships, and reduce the risk of overfitting. It combines multiple decision trees and aggregates their predictions, providing robustness, interpretability, and improved accuracy for predicting flood occurrences based on various factors like rainfall, water levels, and geographical features.
- **Enseble Learning:**
Ensemble learning is used in flood prediction to improve the accuracy and robustness of predictions by combining multiple models. It leverages the diversity of different algorithms or variations of the same algorithm to capture a wider range of patterns, reduce bias, and enhance the overall predictive performance for complex flood prediction tasks.

After comparing all of them, the accuracies were as follows:
<br/>

![Comparison](https://media.discordapp.net/attachments/806974540139200623/1125470919540871238/image.png)

## The Earthquake Prediction Model
**Dataset**
The National Earthquake Information Center (NEIC) determines the location and size of all significant earthquakes that occur worldwide and disseminates this information immediately to national and international agencies, scientists, critical facilities, and the general public. The NEIC compiles and provides to scientists and to the public an extensive seismic database that serves as a foundation for scientific research through the operation of modern digital national and global seismograph networks and cooperative international agreements. The NEIC is the national data center and archive for earthquake information.
[Dataset](https://www.kaggle.com/datasets/usgs/earthquake-database)

**ML Models**
The prediction algorithms that I tested out were: 
- **KNN Classifier:**
The KNN classifier is used in earthquake prediction due to its ability to capture complex and non-linear relationships between various seismic features, such as magnitude, depth, and location. By considering the nearest neighbors to a given earthquake event, KNN can identify patterns and similarities that help predict the likelihood of future earthquakes with similar characteristics.
- **Decision Tree Classification:**
The decision tree classifier is used in earthquake prediction due to its ability to handle complex decision-making processes and capture non-linear relationships between seismic features, such as magnitude, depth, and location. It provides interpretability and can effectively categorize earthquake events based on a series of hierarchical decisions, making it a suitable choice for earthquake prediction tasks.
- **Random Forest Classification:**
The random forest classifier is used in earthquake prediction due to its ability to handle high-dimensional and complex data, capture non-linear relationships, and reduce the risk of overfitting. By combining multiple decision trees and aggregating their predictions, the random forest classifier provides improved accuracy and robustness in predicting earthquake events based on various seismic features such as magnitude, depth, and location.

After comparing all of them, the accuracies were as follows:
<br/>

![Comparison](https://cdn.discordapp.com/attachments/806974540139200623/1125481170411470858/image.png)
## The Hurricane Prediction Model
**Dataset**
The NHC publishes the tropical cyclone historical database in a format known as HURDAT, short for HURricane DATabase. These databases (Atlantic HURDAT2 and NE/NC Pacific HURDAT2) contain six-hourly information on the location, maximum winds, central pressure, and (starting in 2004) size of all known tropical cyclones and subtropical cyclones.

**ML Models**
The prediction algorithms that I tested out were: 
- **Decision Tree Classification:**
The decision tree classifier is used in hurricane prediction due to its ability to handle complex decision-making processes and capture non-linear relationships between meteorological features such as wind speed, pressure, and temperature. It provides interpretability and can effectively categorize hurricane events based on a series of hierarchical decisions, making it a suitable choice for hurricane prediction tasks.
- **Random Forest Classification:**
The random forest classifier is used in hurricane prediction due to its ability to handle complex and high-dimensional data, capture non-linear relationships, and reduce the risk of overfitting. By combining multiple decision trees and aggregating their predictions, the random forest classifier provides improved accuracy and robustness in predicting hurricane occurrences based on various meteorological features such as wind speed, pressure, and temperature.
- **Gaussian Naive Bayes:**
The Gaussian Naive Bayes classifier is used in hurricane prediction due to its simplicity, efficiency, and ability to handle continuous features like wind speed and pressure. It assumes that the features are independent and normally distributed, making it suitable for modeling the probabilistic relationships between meteorological variables in hurricane prediction tasks.
- **Support Vector Machine:**
The Support Vector Machine (SVM) is used in hurricane prediction due to its ability to handle high-dimensional data, capture complex relationships between meteorological features, and provide good generalization performance. It can effectively classify hurricane occurrences based on patterns in the data, making it a valuable tool for predicting hurricanes based on variables such as wind speed, pressure, and temperature.

After comparing all of them, the accuracies were as follows:
<br/>

![Comparison](https://media.discordapp.net/attachments/806974540139200623/1125509811895795722/image.png)

## The Backend
The backend of this project was created using Flask, a Python web framework. After setting up a virtual environment, Flask was installed, and the project structure was organized with directories for application code, static files, and templates.
<br/>

![Directory Structure](https://media.discordapp.net/attachments/806974540139200623/1125490635579867146/image.png)
## The Frontend
The frontend of this project was built with HTML(Hypertext Markup Language) and CSS(Cascading Style Sheets).
## Challenges I ran into
The biggest challenge for me was finding appropriate datasets.I had to struggle for hours to find datasets and then analyse them. I was not able to find real time data for any of these,  Second challenge I faced was, integrating templates with flask, had to debug and google alot.

## Accomplisments that I am proud of
I am proud of getting the best accuracy I could get in the Hurricane Model. The integration part was a dream for me few days back, but I was able to execute it too!

## What I learned
I learned about new technologies that I never tried before.
I learned how to overcome my fears of integrating backend with frontend.
I learned that Artificial Intelligence is capable of doing almost everything.

## What's next for EnvWarn
1. Upgrade the dataset to real time data using Satelite Imaging and APIs.
2. Improving the models and their efficiency
3. Introducing real time alert system if chances of occurence are severe/high.
4. Implementing Donation Services.
5. Improving Visualisation of the data using charts and analysing historical data
6. Issuing preparedness guides for people living in any disaster prone area
7. Integrating the application with various other platforms like Whatsapp to provide notifications the way users like.

## Getting started with the project

- Clone the project and install dependencies
- Activate virtual environment
- Run pip install -r requirements.txt
- Run python prediction.py
- You're Done!