# The Role of Spark in Data Analysis

A significant amount of time for any data scientist or data professional is spent preparing data. Taking raw, unstructured data and converting it into a form that is clean and convenient for a user to confirm. Data is massive today whether it is publicly available or private data used by an enterprise.

On the publicly available data side you have text data like comments, reviews, or tweets which which are left for users on online forums or government reports. On the private side we have purchases, page views, clicks, messages, surveys, or questionnaires to name a few.

We can mine all of this data to draw insights and influence decision making and drive business strategies, or feed it to sophisticated machine learning models to create systems like spam detection or recommendation systems.

To do any of these with data you will need to convert it from its original form - which might be unstructured, messy, and semantically complex - to a form that is easy to understand and consume which does not include anomalies or corrupt data. This is the data processing and preparation which takes 80% of any data professional's time. 

Tasks involving data processing might include:

- Parsing fields from text
- Accounting for missing values
- Identifying and investigating anomalies
- Summarizing using tables and charts

How you go about doing this and which tool you chose to use depends upon the complexity of the data that you're actually dealing with. We can measure data complexity by looking at it's messiness and it's speed of scaling.

### Data In Spreadsheets (Small data, somewhat messy, scales slowly)

- Low data collection frequency (Grows by 10s - 1000s per day)
- Sometimes involves messy manual data collection
- Many files
- Given that the data is small, using tools like Excel you can interact with and explore the data

### Data In Databases (Medium data, clean/high data integrity)

- High frequency of collection (100,000 rows per day)
- Programmatically collected with high data integrity
- Guaranteed ACID Properties
- We can use tools like SQL, Python, Java, R to process the data

### Data In Distributed Computing (Big data, very Messy, quickly scales)

- Very high frequency of data collection (Millions/Billions of rows per day)
- Files stored across a cluster of machines
- Many many files (webpages, log files)
- Requires a distributed computing engine that can process data in parallel across a large number of machines
- We can use Hadoop MapReduce, Spark
