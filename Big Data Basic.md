# Introduction to Big Data

## 1. What is Data?
Data is simply information — numbers, text, images, videos, sensor readings, etc.

**Examples:**
- Mobile photos 📸
- Bank transactions 💳
- Weather readings 🌦

---

## 2. What is Big Data?
**Big Data** means **huge volumes of data** that are so large, fast-growing, and complex that traditional methods (like Excel or a small database) **cannot handle it efficiently**.

**Key Idea:**  
Big Data is not just about **size**, but also:
- **Speed** – data is coming in very fast (e.g., stock market updates every millisecond)
- **Variety** – different types (text, audio, video, logs, sensor data, etc.)

---

## 3. The 5 V’s of Big Data
1. **Volume** – Large amount of data (TB, PB, ZB...)
2. **Velocity** – Speed at which data is generated & processed (real-time or near real-time)
3. **Variety** – Different formats & sources (structured, semi-structured, unstructured)
4. **Veracity** – Data accuracy & trustworthiness
5. **Value** – Useful insights from data

**Example:**  
YouTube:
- Every minute, **500+ hours** of videos are uploaded.
- Data comes from all over the world (variety), uploaded continuously (velocity), and in massive amounts (volume).
- YouTube needs to figure out trending topics (value) and filter fake videos (veracity).

---

## 4. Difference Between Big Data & Simple Data

| **Aspect**     | **Simple Data** (Traditional)            | **Big Data**                               |
|----------------|------------------------------------------|--------------------------------------------|
| **Size**       | MB to GB                                 | TB to PB or more                           |
| **Tools**      | Excel, SQL databases                     | Hadoop, Spark, NoSQL                       |
| **Processing** | Batch processing, handled on one PC      | Distributed processing over many computers |
| **Structure**  | Mostly structured (tables)               | Structured, semi-structured, unstructured  |
| **Speed Need** | Normal                                   | Often real-time or high-speed              |
| **Storage**    | Local disk                               | Distributed storage (cloud, clusters)      |

**Examples:**
- **Simple Data**: A shop’s monthly sales data (easily fits in Excel)
- **Big Data**: Amazon’s sales data from millions of customers updated every second

---

# Introduction to Hadoop

## 1. Why Hadoop?
Traditional databases fail with Big Data because:
- Data is too **huge** for one machine.
- Processing is too **slow** on a single system.
- Need to handle **different formats** of data.

---

## 2. What is Hadoop?
Hadoop is an **open-source framework** used to store and process Big Data in a **distributed** way across many computers.

> Instead of one supercomputer, use 1000 normal computers working together.

---

## 3. Features of Hadoop
- **Scalable** – Can add more computers easily
- **Fault Tolerant** – If one computer fails, others take over
- **Cost-Effective** – Uses normal hardware (commodity machines)
- **Handles Variety** – Works with structured, semi-structured, and unstructured data

---

## 4. Main Components of Hadoop

### 4.1 HDFS (Hadoop Distributed File System)
Stores data in chunks across multiple computers.  
Example: A 100 MB file may be split into 3 parts and stored on different computers for safety.

### 4.2 MapReduce
The processing engine that divides tasks into smaller parts and runs them in parallel.  
Example: Count words in a huge book by splitting it into parts, counting each part separately, then combining results.

### 4.3 YARN (Yet Another Resource Negotiator)
Manages resources and schedules jobs in Hadoop.  
Example: Decides which computer will run which task.

---

## 5. Hadoop Ecosystem Tools
- **Hive** – SQL-like queries for Big Data
- **Pig** – Script-based data processing
- **HBase** – NoSQL database for Big Data
- **Sqoop** – Transfer data between Hadoop and traditional databases
- **Flume** – Import streaming data (like logs) into Hadoop
- **Tez**   - A framework to build **fast and efficient** data processing applications on top of Hadoop. It improves MapReduce by enabling complex task graphs and reduces disk I/O for better performance.  
- **Spark** - An **in-memory distributed data processing engine** faster than MapReduce. Supports batch and real-time processing with libraries for SQL, machine learning, graph processing, and streaming.  
- **Mesos** - A **cluster resource manager** that shares CPU, memory, and storage efficiently across multiple distributed frameworks like Hadoop and Spark.
- **Oozie** - A **workflow scheduler** that automates running complex Hadoop job sequences based on time or data availability.  
- **Zookeeper** - A **distributed coordination service** managing configuration, synchronization, and leader election in distributed systems.  
- **Storm** - A **real-time stream processing system** that processes continuous data streams instantly.  

---

## Summary
- **Big Data** = Large, fast, varied data that traditional tools can’t handle.  
- **Difference** = Big Data needs distributed tools; small data can work with normal tools.  
- **Hadoop** = Framework for storing & processing Big Data across multiple machines efficiently.  
- **Architecture** = Master-Slave design with HDFS, YARN, MapReduce, and ecosystem tools.  
- **Other Tools** = Tez, Spark, Mesos, Oozie, Zookeeper, and Storm add speed, resource management, workflow scheduling, coordination, and real-time processing to the ecosystem.
