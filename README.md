<!-- Add logo -->
<!--  ![App Logo](https://i.stack.imgur.com/ARgpq.jpg) -->


[![forthebadge](https://forthebadge.com/images/badges/built-by-developers.svg)](https://forthebadge.com)
[![pythonbadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)

# 📱 Data Storyteller 📉

_**ONE STOP SOLUTION FOR ALL YOUR DATA NEEDS**_ 
## Introduction 

As per Gartner, the analytics and business intelligence platform market has transitioned from the visual data discovery era to the augmented era. Data and analytics leaders/administrators should begin piloting capabilities and competencies that enable the “augmented consumer”.

With the technology advancements, the organisation today has the pre-eminence of taking data driven decisions and strategize their planning, forecasts based on the same. A profusion of business users do not have time to analyze the data and then secure noteworthy insights. And there are gaps betwixt how the tool produces an output and how the business user can exploit it to interpret it. In accompaniment, it needs a admirable domain knowledge to build business insights from data. Not every user is a business expert. Given a snapshot of data, we would like to fabricate a system which can verbalise a story from the data. The story includes the automation in the sense of being driven by the data, context and personal preferences. In this case, it solves both the problems of the tool usage as well as guiding the user with the data driven intelligence to make business decision. The whole corollary is driven by outcome and effectiveness.

## Tool Description 

Data Storyteller is an AI based tool that can take a data set, identify patterns in the data, can interpret the result, and can then produce an output story that is understandable to a business user based on the context. It is able to pro-actively analyse data on behalf of users and generate smart feeds using natural language generation techniques which can then be consumed easily by business users with very less efforts. The application has been built keeping in mind a rather elementary user and is hence, easily usable and understandable. This also uses a **multipage implementation** of Streamlit Library using Class based pages. 

## Features 

Given data/analytics output, the tool can:-

- turn the data into interactive data stories based on the given data 
- generate deep insights, infer pattern and help in business decisions.
- provide personalization profiles; these could be represented as meta data describing what would be of interest to a given user.
- generate reports understandable to a business user with interactive and intuitive interface.

## 📝 Module-Wise Description

The application also uses Streamlit for a multiclass page implementation which can be viewed in the `multipage.py` file. The UI of the application can be seen here. The application is divided into multiple modules, each of which have been described below.

![UI of the application](https://i.stack.imgur.com/MOVpz.png)


_📌 **Data Upload**_ <br/>

This module deals with the data upload. It can take csv and excel files. As soon as the data is uploaded, it creates a copy of the data to ensure that we don't have to read the data multiple times. It also saves the columns and their data types along with displaying them for the user. This is used to upload and save the data and it's column types which will be further needed at a later stage. 

_📌 **Change Metadata**_ <br/>

Once the column types are saved in the metadata, we need to give the user the option to change the type. This is to ensure that the automatic column tagging can be overridden if the user wishes. For example a binary column with 0 and 1s can be tagged as numerical and the user might have to correct it. The three data types available are:

* Numerical 
* Categorical 
* Object

The correction happens immediately and is saved at that moment. 

_📌 **Machine Learning**_ <br/>

This section automates the process of machine learning by giving the user the option to select X and y variables and letting us do everything else. The user can specify which columns they need for machine learning and then select the type of process - regression and classficiation. The application selects multiple models and saves the best one as a binary `.sav` file to be used in the future for inferencing. The accuracy or R2 score is shown right then and there with the model running in the background.  

_📌 **Data Visualization**_ <br/>

_📌 **Y-Parameter Optimization**_ <br/>

## Technology Stack 

1. Python 
2. Streamlit 
3. Pandas
4. Scikit-Learn
5. Seaborn

# How to Run 

- Clone the repository
- Setup Virtual environment
```
$ python3 -m venv env
```
- Activate the virtual environment
```
$ source env/bin/activate
```
- Install dependencies using
```
$ pip install -r requirements.txt
```
- Run Streamlit
```
$ streamlit run app.py
```



## 🤝 How to Contribute? [3]

- Take a look at the Existing Issues or create your own Issues!
- Wait for the Issue to be assigned to you after which you can start working on it.
- Fork the Repo and create a Branch for any Issue that you are working upon.
- Create a Pull Request which will be promptly reviewed and suggestions would be added to improve it.
- Add Screenshots to help us know what this Script is all about.


# 👨‍💻 Contributors ✨

<table>
  <tr>
    <td align="center"><a href="https://github.com/vishalsingh17"><img src="https://avatars.githubusercontent.com/u/55878408?s=400&u=55bd0c70828a4fe8b828ac3f9099ec7faa1b9593&v=4" width="100px;" alt=""/><br /><sub><b>Vishal Singh</b></sub></a><br /></td>
    <td align="center"><a href="https://github.com/ashishgarg052"><img src="https://avatars.githubusercontent.com/u/48443496?v=4" width="100px;" alt=""/><br /><sub><b>Ashish Garg</b></sub></a><br /></td>

</table>

## References 

[1] SAP Hackathon: https://sap-code.hackerearth.com/challenges/hackathon/sap-code/custom-tab/data-4-storytelling/#Data%204%20Storytelling (used for the `README.md` introduction)

[2] Gartner: https://www.gartner.com/en/documents/3982132

[3] Soumyajit Behera: https://github.com/soumyajit4419/MedHub_360


## Contact

For any feedback or queries, please reach out to [vishal170997@gmail.com](vishal170997@gmail.com).

Note: The project is only for education purposes.
