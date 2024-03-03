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

To do so, we will be taking the help of **Alteryx**. For those who is new to ALteryx, a lttle bit context: _Alteryx is a software solution that allows users to quickly access, manipulate, analyze, and output data. The software is designed to make advanced analytics automation accessible to any data worker._
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

- We have left the null values as in alteryx we can perform the analysis without using them. Cleanse and standardize text fields such as titles, directors, and cast by removing leading/trailing spaces, converting to lowercase, or addressing inconsistencies.
- We have selected the columns which will be need to perform the data analysis.
- Duplicates can distort analysis results, so it’s essential to address them. As the primary key is the show_id. Using the unique tool, all the duplicate value will be removed.

 The data after cleaning:
 
 <img width="893" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/124201c8-a719-434f-8134-7236a05a1cee">

***
## Data Analysis 
### Distribution of the Content Type 

- To determine the distribution of content in the Netflix library, we will use Summarize and Interactive chart tool.
- In Summarize tool, configure the Summarize tool to group by the "type" column. Then, choose the "Count" aggregation method to count the occurrences of each type.
<img width="294" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/d1c01447-0543-4f89-84fa-bb66bca451c1">

The pie chart visualization shows that approximately 70% of the content on Netflix consists of film, while the remaining 30% are TV shows.
### Which countries creates the most content?
 
- Next, let us identify the top 10 countries where Netflix is popular.
- In Summarize tool, configure the Summarize tool to group by the "country" column. Then, choose the "Country" aggregation method to count the occurrences of each type.
- Then, arrange it in descending order using the "Sort" which will give me the top 10 countries with highest number of content in the library.
- Finally, using the "interactive graph" to visualize the results.

<img width="403" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/48561022-edbc-46bd-94f4-0b57f27465d9">

The most prolific producers of content for Netflix are the United States, India, and United Kingdom. Numerically, although India and the U.K. rank second and third among Netflix content producers, they have a significant distance behind the U.S. 

### Who has directed the most content in Netflix?

- Now, let us identify the top directors who have directed the highest number of movies or TV shows according to the netflix library.
  

<img width="230" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/131a1b3b-2050-4f69-bbd9-a99828674b93">

### How old is the content in the Netflix library?

- Netflix’s success lies in promoting a mix of both ‘old-fashioned’ content and radical advancements.
<img width="344" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/50af9d46-d201-4418-8bb7-1af9f5b3096c">


### Who is the target audience of Netflix?
- Some ratings are only applicable to Movies, such as PG-13, PG, NC-17, and UR. The largest groups of target audience are Adults and Teenagers, aligning with TV-MA & R ratings for adults and TV-14 & PG-13 ratings for teens — 4 in 5 most common ratings of Netflix content.
  
<img width="134" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/6a13da4e-7a3a-412a-80f6-5146e6f591a2">


### How long is the content in Netflix library?

<img width="200" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/6da3bce0-7a22-4569-be22-70bb40c7a6d4">

<img width="338" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/353306ef-3296-4843-a6a2-539cee5b719e">




### Which genre is more popular?

- Netflix offers a range of genres to subscribers, and it would be interesting to analyze this feature. One thing to notice is that most of Movie content falls into multiple genres.
<img width="239" alt="image" src="https://github.com/pankhuridata/Netflix-Using_Alteryx/assets/109762146/a678def3-e625-4eeb-add8-d4a1663affd7">
