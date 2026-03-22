# 🏭 FMCG Data Engineering Project
### AWS + Databricks + Apache Spark | Medallion Architecture

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)
![Apache Spark](https://img.shields.io/badge/PySpark-E25A1C?logo=apachespark&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-S3-FF9900?logo=amazonaws&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Overview

A real-world FMCG pipeline simulating a company acquisition scenario — consolidating data from two companies with different schemas into a single source of truth using a **hybrid AWS + Databricks Lakehouse architecture**.

> 📺 Inspired by [Codebasics Data Engineering Tutorial](https://www.youtube.com/@codebasics)

---

## 🏗️ Architecture

```
Source Data ──► Amazon S3 ──► 🥉 Bronze ──► 🥈 Silver ──► 🥇 Gold
                (Raw Lake)      (Raw ingest)  (Clean+Join)  (BI-ready)    
                                    Databricks + PySpark                        
                                  
```
# 🔧 Tech Stack

| Layer | Tools |
|-------|-------|
| Cloud Storage | Amazon S3|
| Transformation | Databricks, Apache Spark, PySpark |
| Architecture | Medallion (Bronze / Silver / Gold) |
| Languages | Python, SQL |
---

## 🔄 Pipeline Steps

1. **S3** — Raw CSV/JSON from both companies landed in the data lake
2. **Bronze** — Autoloader ingests data as-is into Delta tables
3. **Silver** — PySpark cleans, deduplicates, and joins both company datasets
4. **Gold** — Aggregated, business-ready tables for reporting

---

## 💡 Key Learnings

- Designing a hybrid AWS + Databricks pipeline from scratch
- Medallion Architecture as an industry standard for data lakes
- Merging multi-source data with different schemas via PySpark
---


## 🙏 Credits
Tutorial by *Dhaval Patel — Codebasics*

---

## 👤 Author

**Divy Shukla**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?logo=linkedin)](https://www.linkedin.com/in/divy-shukla123/)

⭐ *If this was helpful, drop a star!*
