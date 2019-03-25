# Understanding The Components Of Spark

Spark is an engine for data processing and analysis. This engine has three important characteristics that make it perfect for dealing with big data. It is **general purpose**, **interactive**, and **utilizes distributed computing**.

It is general purpose because the same engine can be used for doing multiple things with data like: Exploring, Cleaning and Preparing, Applying Machine Learning, Building Data Applications. 

Spark also has interactive environments where you can type in a command and see its results immediately. These environments are called **REPL** which stands for **Read, Evaluate, Print, Loop**. Spark's built-in REPL environments for both Scala and Python provide fast feedback and allow you to iterate very quickly to do your explorations. 

*Spark is a distributed computing engine* - meaning it processes data across a number of machines and it can be integrated with other distributed computing engines like Hadoop.

To work with Spark you use the **Spark APIs**. These APIs are built in Scala but can be accessed using Scala, Python, or Java.

***

## How We Use Data In Spark

Almost all data is processed using **Resilient Distributed Datasets** (RDDs). They are the main programming abstraction in Spark. Using RDDs, Spark loads data into memory and then processes it. RDDs are in-memory collections of objects. Each object in the collection represents one record in your dataset and all the records in the dataset are kept in memory across a cluster of machines. What makes RDDs useful is that they are in-memory yet resilient - meaning they are tolerant to falls or crashes. With RDDs you can interact and play with billions of rows of data scored across a cluster of machines without caring about any of the complexities involved in resource management or fault tolerance. 

***

## The Three Components Of Spark

Spark is made up of three components: **Spark Core, Storage System, Cluster Manager**

Spark Core handles the basic functionality of Spark, including creating and processing RDDs. In addition to Spark Core, Spark needs two additional components because otherwise it is just a computing engine. Spark Core needs to connect with a **Storage System** that can store the data it will process and a **Cluster Manager** that will help Spark to run and schedule tasks across a cluster of machines. Both of these components can actually plug and play. For the *Storage System*, you can choose between your local file system (Used in standalone mode) or HDFS (Integration with Hadoop). For the Cluster Manager you can use Spark's own built-in cluster manager (Comes in standalone mode) or you can plug in Yarn if you're integrating with Hadoop.
