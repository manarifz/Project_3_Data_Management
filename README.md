# 🎬 MovieLens 100k Data Exploration with Spark SQL & Apache Zeppelin

This project utilizes Apache Zeppelin and Spark SQL to analyze the MovieLens 100k dataset, focusing on user behavior, movie preferences, and demographic insights. The goal is to answer specific analytical questions and demonstrate the integration of Spark with modern data tools.

> Dataset can be obtained from [MovieLens 100k Dataset](https://grouplens.org/datasets/movielens/100k/)

## 🔍 Project Summary

The MovieLens 100k dataset contains 100,000 ratings from 943 users across 1,682 movies. Through this project, we use Spark SQL to uncover patterns and answer the following:

1. 📊 What is the average rating for each movie?

2. 🏆 Which 10 movies have the highest average ratings?

3. 🎯 Which users have rated at least 50 movies, and what are their favorite genres?

4. 👶 Who are the users younger than 20 years old?

5. 🧪 Which users are scientists aged between 30 and 40?

## 🧰 Tools & Technologies Used
![Hadoop Ecosystem](https://img.shields.io/badge/Hadoop%20Ecosystem-660000?style=flat&logo=apache-hadoop&logoColor=white)
![Spark](https://img.shields.io/badge/Apache%20Spark-FF3333?style=flat&logo=apache-spark&logoColor=white)
![Zeppelin](https://img.shields.io/badge/Apache%20Zeppelin-003F7D?style=flat&logo=apache-zeppelin&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-006F9C?style=flat&logo=sql&logoColor=white)

- **Apache Zeppelin**: For interactive notebook interface for data analysis.
- **Apache Spark SQL**: For querying and processing the dataset.
- **ML-100k Dataset**: Core dataset for the analysis.

## 🗃️ Dataset Description

- `u.data`: Ratings (userID, movieID, rating, timestamp).
- `u.item`: Movies metadata (movieID, title, genre).
- `u.user`: User info (userID, age, gender, occupation, zip code).

## ✅ Tasks Performed

1. **Calculate the average rating for each movie**:
   - Aggregate the ratings for each movie and calculated the average.

2. **Identify the top 10 movies with the highest average ratings**:
   - Sort the movies based on their average ratings in descending order.

3. **Find the users who have rated at least 50 movies and their favourite genres**:
   - Filter users who have rated 50 or more movies, then identified their favorite movie genres based on their ratings.

4. **Find all the users who are less than 20 years old**:
   - Filter users by age to identify those younger than 20.

5. **Find all the users whose occupation is "scientist" and whose age is between 30 and 40 years old**:
   - Filter users based on occupation and age range.

## ⚙️ Setup & Execution

### 📌 Prerequisites
1. **Hadoop Ecosystem**: Make sure the hadoop ecosystem is set up.
2. **Apache Zeppelin**: Make sure Apache Zeppelin is installed and running.
3. **Spark**: Ensure Spark is installed and configured with Zeppelin.


### 🛠️ Steps to Execute:

1. Download the dataset or use the script below.
2. Load files (u.data, u.item, u.user) into /tmp directory or HDFS.
3. Open Apache Zeppelin and import the notebook.
4. Run Spark SQL queries to perform analysis.

> 📥 Download Data via Shell Script:

```shell
wget http://media.sundog-soft.com/hadoop/ml-100k/u.user -O /tmp/u.user
wget http://media.sundog-soft.com/hadoop/ml-100k/u.data -O /tmp/u.data
wget http://media.sundog-soft.com/hadoop/ml-100k/u.item -O /tmp/u.item
```
