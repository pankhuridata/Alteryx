# Netflix Case Study: EDA using Alteryx 
![seo-watch-free-link-preview](https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/dfee43a4-05c0-4466-a5ed-5db3909e5d5d)

***
## Table of Contents
- [Introduction](#Introduction)
- [About the Data](#About-the-Data)
- [Data Preparation](#Data-Preparation)
- [Data Analysis](#Data-Analysis)

Dataset Link: [here](https://www.kaggle.com/datasets/shivamb/netflix-shows)
***
## Introduction
When we think about streaming platform, the first name that comes to our mind is Netflix. Netflix has revolutionized the entertainment industry with its streaming platform. But behind this success lies a powerful data engine that drives content acquisition, recommendation algorithms, and user engagement. This project delves into the world of Netflix data, exploring insights hidden within content trends and platform performance.

To do so, I will be taking the help of **Alteryx**. For those who is new to ALteryx, a lttle bit context: _Alteryx is a software solution that allows users to quickly access, manipulate, analyze, and output data. The software is designed to make advanced analytics automation accessible to any data worker._
> Alteryx also host weekly challenges which can help in knowing more about this amazing data analytics software. The link is [here](https://community.alteryx.com/t5/Weekly-Challenge/bd-p/weeklychallenge)
***
## About the Data
First, let’s take a look at the dataset.

Netflix dataset consists of _8,807 rows_ of movies and TV shows and _12 columns_ providing 12 characteristics for each movie/TV show. Here is a table summarizing the columns and their description:

<img width="306" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/01a6ad12-4167-4dd1-a40f-23f3d93079b4">

***
## Data Preparation
In this section, we will perform data preparation tasks onthe Netflix dataset to ensure its cleanliness and suitability for analysis. We will handle missing values and duplicates and perform data type conversions as needed.
<img width="188" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/8c81631d-998a-49f9-8755-80fc2861dabb">

- I have left the null values as in alteryx we can perform the analysis without using them.
- I have selected the columns which will be need to perform the data analysis.
- Duplicates can distort analysis results, so it’s essential to address them. As the primary key is the show_id. Using the unique tool, all the duplicate value will be removed.

 The output is:
  <img width="893" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/124201c8-a719-434f-8134-7236a05a1cee">
