# 🎬 Project 3 - MovieLens Data Management Assignment

**👤 Author:** <Your Name>  
**🏫 Course:** STQD6324 Data Management (Sem 2, 2024/2025)  
**⏰ Deadline:** June 28, 2025

---

## 🔎 Brief
Build an **end-to-end pipeline** that ingests, processes, and analyzes the MovieLens 100k dataset using Hadoop, Spark, and Cassandra. Gain hands-on experience with distributed storage, big-data processing, and NoSQL querying. 🤓

---

## 📖 Project Overview
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
1. **⭐ Average rating per movie**  
2. **🏆 Top 10 movies by highest average rating**  
3. **🎯 Users with ≥ 50 ratings & their favorite genres**  
4. **👶 Users under 20 years old**  
5. **🔬 Scientists aged 30–40**

---

## 🚀 Setup Instructions
1. **Clone the repo**  
   ```bash
   git clone https://github.com/<username>/movielens-assignment3.git
   cd movielens-assignment3
