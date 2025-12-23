# ✈️ Airline Analytics Dashboard

##  Project Overview
This project focuses on analyzing airline flight data to evaluate operational performance, delays, cancellations, and overall efficiency.  
The goal is to transform raw flight data into meaningful insights using data engineering and business intelligence tools.

## Objectives
- Analyze flight delays and cancellations
- Measure airline operational efficiency
- Identify patterns in on-time performance
- Build an interactive dashboard for decision-makers

> **Data Source:** 
    Kaggle Dataset: "Flight Delays and Cancellations"
    URL: https://www.kaggle.com/datasets/usdot/flight-delays
    Files:
      - flights.csv (main dataset)
      - airlines.csv (airline codes)
      - airports.csv (airport codes)
> ## Dataset
The dataset includes the following key fields:
- Flight Date
- Airline
- Flight Number
- Origin & Destination
- Departure Delay
- Arrival Delay
- Cancellation Status
- Diversion Status
- Flight Duration

## Tools & Technologies
- **Java** (for pyspark installation)
- **Apache Spark** (for pyspark installation)
- **Python** (PySpark)
- **SQL** (Data storage)
- **Power BI** (Dashboard & visualization)

## Key Metrics
- On-Time Performance (%)
- Average Departure Delay
- Average Arrival Delay
- Cancellation Rate
- Diversion Rate
- Total Flights per Airline

## Project One-by-One Description.

## 📂 Datasets
All datasets used in this project were downloaded from **Kaggle**.

🔗 Kaggle Platform:  
https://www.kaggle.com

> A free Kaggle account is required to download datasets.

---

## 🧰 Environment Setup (PySpark on Windows)

This project uses **PySpark** for data processing.  
Follow the steps below to configure the required environment.

---

### ☕ 1. Install Java (JDK)
PySpark requires Java to be installed.

**Recommended versions:** JDK 11 or JDK 8

🔗 Oracle JDK 11 (Archive):  
https://www.oracle.com/java/technologies/javase/jdk11-archive-downloads.html

🔗 OpenJDK (Free alternative):  
https://adoptium.net

**After installation:**
- Set environment variable:
  ```text
  JAVA_HOME = C:\Program Files\Java\jdk-11
  ```

* Add to PATH:
  ```text
  %JAVA_HOME%\bin
  ```

### ⚡ 2. Install Apache Spark

**Version used:** Spark 3.5.7
**Package:** spark-3.5.7-bin-hadoop3.tgz

🔗 Download Spark:
[https://spark.apache.org/downloads.html](https://spark.apache.org/downloads.html)

**Steps:**

1. Extract Spark to:

   ```text
   C:\spark
   ```
2. Set environment variable:

   ```text
   SPARK_HOME = C:\spark
   ```
3. Add to PATH:

   ```text
   %SPARK_HOME%\bin
   ```

---

### 🐘 3. Install Hadoop (winutils.exe)

Windows requires `winutils.exe` for Hadoop compatibility.

🔗 Download winutils.exe:
[https://github.com/cdarlint/winutils](https://github.com/cdarlint/winutils)

**Steps:**

1. Create folders:

   ```text
   C:\hadoop\bin
   ```
2. Place `winutils.exe` inside `bin`
3. Set environment variable:

   ```text
   HADOOP_HOME = C:\hadoop
   ```
4. Add to PATH:

   ```text
   %HADOOP_HOME%\bin
   ```

---

### 🐍 4. Install Python

**Version used:** Python 3.11.x (Recommended)

🔗 Download Python:
[https://www.python.org/downloads/](https://www.python.org/downloads/)

**Important during installation:**

* ✅ Check **Add Python to PATH**

**Verify installation:**

```bash
python --version
pip --version
```

---

### 🐘 5. Install PostgreSQL & pgAdmin

PostgreSQL is used as the project database.

🔗 Download PostgreSQL (includes pgAdmin):
[https://www.postgresql.org/download/windows/](https://www.postgresql.org/download/windows/)

**Steps:**

* Install PostgreSQL
* Set database username and password
* pgAdmin will be installed automatically

---

### 📦 6. Install PySpark

Install PySpark using pip:

```bash
pip install pyspark==3.5.7
```

**Verify PySpark:**

```bash
pyspark
```

---

## 🗂 Recommended Folder Structure

```text
C:\
├── spark\
├── hadoop\
│   └── bin\
│       └── winutils.exe
├── data\
│   ├── raw\
│   └── processed\
├── scripts\
└── notebooks\
```

---

## 🔧 Environment Variables Summary

| Variable    | Value                                                      |
| ----------- | ---------------------------------------------------------- |
| JAVA_HOME   | C:\Program Files\Java\jdk-11                               |
| SPARK_HOME  | C:\spark                                                   |
| HADOOP_HOME | C:\hadoop                                                  |
| PATH        | %JAVA_HOME%\bin;<br>%SPARK_HOME%\bin;<br>%HADOOP_HOME%\bin |









