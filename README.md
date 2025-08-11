# Big-Data-Lab


Introduction to Big Data
1. What is Data?
Data is simply information in various forms—numbers, text, images, videos, sensor readings, etc.

Examples:

Mobile photos 📸

Bank transactions 💳

Weather readings 🌦

2. What is Big Data?
Big Data refers to extremely large and complex datasets that traditional tools like Excel or small databases cannot handle efficiently.

Key points:
Size: Huge volumes of data (terabytes, petabytes, or more)

Speed: Data generated and processed rapidly (e.g., stock prices updated every millisecond)

Variety: Data comes in many types — text, audio, video, logs, sensor data, and more

3. The 5 V’s of Big Data
V	Meaning	Explanation
Volume	Large amount of data	Terabytes, Petabytes, Zettabytes
Velocity	Speed of data generation and processing	Real-time or near real-time flow
Variety	Different data types and formats	Structured, semi-structured, unstructured
Veracity	Accuracy and trustworthiness of data	Data quality and reliability
Value	Meaningful insights extracted	Business or operational benefits

Example: YouTube

500+ hours of videos uploaded every minute (Volume & Velocity)

Videos from worldwide users in different formats (Variety)

Detects trending content (Value)

Filters out fake videos (Veracity)

4. Difference Between Big Data & Simple Data
Aspect	Simple Data	Big Data
Size	Megabytes to Gigabytes	Terabytes to Petabytes or more
Tools	Excel, SQL Databases	Hadoop, Spark, NoSQL databases
Processing	Batch processing on a single PC	Distributed processing over many machines
Structure	Mostly structured (tables)	Structured, semi-structured, unstructured
Speed	Normal speed	Often real-time or high-speed
Storage	Local disk	Distributed storage (cloud, clusters)

Example:

Simple Data: Monthly sales data for a small shop

Big Data: Amazon’s sales data from millions of customers updated continuously

Introduction to Hadoop
1. Why Hadoop?
Traditional databases struggle with Big Data because:

Data volume is too large for a single machine

Processing is too slow on one system

Data formats are diverse and complex

2. What is Hadoop?
Hadoop is an open-source framework designed to store and process Big Data in a distributed manner across many computers.

Think: Instead of one powerful machine, Hadoop uses thousands of ordinary computers working together.

3. Features of Hadoop
Scalable: Easily add more computers to handle growing data

Fault-tolerant: If one machine fails, others continue working

Cost-effective: Uses inexpensive commodity hardware

Flexible: Handles structured, semi-structured, and unstructured data

4. Main Components of Hadoop
4.1 HDFS (Hadoop Distributed File System)
Splits and stores data chunks across multiple machines for reliability and speed.
Example: A 100 MB file split into parts stored on different computers.

4.2 MapReduce
Processes large data by dividing tasks into smaller chunks that run in parallel, then combines results.
Example: Counting words in a huge book by splitting it and processing each part simultaneously.

4.3 YARN (Yet Another Resource Negotiator)
Manages system resources and schedules tasks on the cluster machines.

5. Hadoop Ecosystem Tools
Hive: SQL-like querying language for Big Data

Pig: Script-based data transformation tool

HBase: NoSQL database for Big Data storage

Sqoop: Transfers data between Hadoop and traditional databases

Flume: Collects and imports streaming data (e.g., logs)

Tez: Enhances MapReduce by enabling faster and more complex data processing workflows

Spark: In-memory data processing engine for batch & real-time data, faster than MapReduce

Mesos: Efficient resource manager sharing CPU, memory, storage across frameworks

Oozie: Workflow scheduler for automating complex job sequences

Zookeeper: Coordinates distributed systems with configuration, synchronization, leader election

Storm: Processes real-time streaming data continuously

Summary
Big Data: Large, fast, and varied data that traditional tools can’t handle efficiently.

Hadoop: Open-source distributed framework to store and process Big Data across many machines.

Architecture: Master-slave model with HDFS for storage, YARN for resource management, MapReduce for processing.

Ecosystem: Includes tools for querying, resource management, streaming, scheduling, and coordination to enhance Big Data processing.
