# 🎬 Project 3 - MovieLens Data Management Assignment

**👤 Author:** Muhammad Zuhair Afham Bin Mohd Nasir
**🏫 Course:** STQD6324 Data Management (Sem 2, 2024/2025)  
**⏰ Deadline:** June 28, 2025

---
![MovieLens Pipeline Overview](https://bookandfilmglobe.com/film/my-life-as-a-movielens-test-subject/)


## 📖 Project Overview

This project ingests the MovieLens 100k dataset into HDFS and Cassandra, transforms it with Spark, and analyzes user ratings and demographics using Spark SQL and Cassandra CQL. 🤓

- **📥 Load:** MovieLens data into HDFS and Cassandra.  
- **🔄 Transform:** Raw files into Spark DataFrames/RDDs and persist results.  
- **📊 Analyze:** Ratings and user behavior via Spark SQL and Cassandra CQL.  
- **📝 Document:** Each step in scripts and a Jupyter notebook for reproducibility.

---

## 🛠️ Tools & Technologies
- **Hadoop/HDFS**: Distributed file storage. 💾  
- **Apache Spark (2.x)**: Data processing engine. ⚡  
- **Apache Cassandra**: NoSQL database for scalable reads/writes. 📚  
- **Python 3.x**: `pyspark`, `cassandra-driver`, `argparse`. 🐍  
- **Jupyter Notebook**: Interactive exploration and reporting. 📓

---

## 🗂️ Dataset
- **u.user (Users):** 943 records with `user_id | age | gender | occupation | zip`. 👥  
- **u.item (Movies):** 1,682 records with `movie_id | title | release_date | genre flags`. 🎥  
- **u.data (Ratings):** 100,000 records with `user_id   movie_id   rating   timestamp`. ⭐

---

## ❓ Questions / Tasks
1. ** Calculate the average rating for each movie.**
2. ** Identify the top ten movies with the highest average ratings.**
3. ** Find the users who have rated at least 50 movies and identify their favourite movie genres.**  
4. ** Find all the users who are less than 20 years old.**  
5. ** Find all the users whose occupation is “scientist” and whose age is between 30 and 40 years old.**

---

## 🚀 Setup Instructions
1. **Clone the repo**  
   ```bash
   git clone https://github.com/<username>/movielens-assignment3.git
   cd movielens-assignment3
   
2. **Upload Data in Zeppelin**

- **Open Apache Zeppelin in your browser.**
- **Upload the provided JSON/script into a new notebook.**
- **Fetch Raw Dataset.**
  ```bash
   wget http://media.sundog-soft.com/hadoop/ml-100k/u.user   -O /tmp/u.user
   wget http://media.sundog-soft.com/hadoop/ml-100k/u.data   -O /tmp/u.data
   wget http://media.sundog-soft.com/hadoop/ml-100k/u.item   -O /tmp/u.item
