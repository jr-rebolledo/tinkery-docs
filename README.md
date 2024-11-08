# Tinkery Docs

## Index

* [Quick Setup](https://github.com/jr-rebolledo/tinkery-docs/blob/main/README.md)
* [Glossary](#Glossary)
* [Your First Tinkery Project](#YourFirstTinkeryProject)
* [Uploading Files](#UploadingFiles)
* [Connecting Data Sources](#ConnectingDataSources)
* [Tinkery AI](#TinkeryAI)
* [Prompting Guidelines](#PromptingGuidelines)

## Quick Setup Instructional Guide for Tinkery

Tinkery is an intelligent analytical warehouse designed for non-technical users in fields like customer experience, marketing, and sales. This guide will walk you through the steps of setting up Tinkery and using its features for the first time.

#### Step 1: Sign Up and Log In
Sign Up: Navigate to Tinkery's homepage and click on the "Sign Up" button. Follow the prompts to create your account.
Log In: After confirming your email, log into Tinkery using your credentials.

#### Step 2: Connect or Upload Your Data
Connect Data: Choose to connect your data from various sources (e.g., CRM, marketing platforms, or sales databases) by following the on-screen prompts.
Upload Data: Alternatively, upload files directly into Tinkery. Supported formats include CSV, JSON, and Excel.
Receive success notification: Once the connection to your data source is achieved, or your file located and uploaded, a confirmation message will appear.

#### Step 3: Create Data Domain Projects
Name Your Project: Try to name your project something that reflects what the project is trying to achieve.
Eg. A project trying to understand customer lifetime value per industry could be called, “CLV per Industry”.
Provide Context: Once connected or uploaded, Tinkery will ask you to describe the data (e.g., "This dataset contains customer purchase history" or "Marketing campaign performance"). This context helps Tinkery create metadata for better analysis.
Select Data: This is where Tinkery allows you to organize and contextualize your data sources. Go through the list of data sources available, and locate the files, tables, collections that you want to add to this project. Add natural language descriptions to each of your datasets. These should be descriptions of what those tables and files contain.
Eg. “This table contains all vehicles driving into the main factories plants in the past 3 years, it holds times they entered and exited as well as specific details of the vehicles”
Build Relationships: Tinkery will now automatically create relationships between them using context-driven ontologies. All this data will allow you to explore, query, visualize and predict data.
Review Ontologies: These relationships will be stored as ontologies, which you can later use to query and transform your data. These will be displayed for you in the project creation wizard and can be manually edited.

#### Step 4: Generate Metadata
Tinkery's AI: Using foundational models, Tinkery automatically generates metadata for your connected or uploaded data. This metadata will later help in data cleaning, analysis, and creating relations between datasets. You can choose to allow Tinkery to create domain related features which can be invaluable for further analysis.

#### Step 5: Clean and Modify Data
Explore Data: Once the metadata is generated, you can begin cleaning your data in Tinkery’s AI interface.
Identify Issues: Tinkery can identify missing or bad-quality data.
Modify Data: Accept Tinkery's suggestions for best practices in cleaning the data (e.g., filling missing fields or correcting inconsistencies). If you are not sure how to proceed with your data cleaning, just ask Tinkery.
Manual Adjustments: You can also manually modify your data where necessary, following the suggested best practices.

#### Step 6: Query, Explore, and Transform Your Data
Natural Language Interface: Use Tinkery’s natural language interface to query your data. For example, you can ask, "Show me the top 10 customers by purchase amount last quarter," and Tinkery will generate a response based on the data relationships it has created.
Explore: Dive deeper into your data by asking follow-up questions or refining your queries. Exploring is more about you figuring what you want to ask, Tinkery will make you forget about the how.
Transform: Apply transformations to your data using natural language commands, allowing you to extract actionable insights. Leveraging features already created or building new ones, you can transform your data into new valuable datasets.

#### Step 7: Leverage Metadata Across Services
The metadata generated by Tinkery can be leveraged by other services in your organization, making it easier to integrate and collaborate across teams.

#### Step 8: Collaborate and Share Insights
Collaborate: Share data projects and insights with other team members. Tinkery’s intuitive interface allows for easy collaboration without needing technical expertise.
Export Results: Export your analysis and visualizations to share reports with stakeholders or other departments.

_Last update 8 November 2024_




## Glossary

### -> Introduction to Tinkery

### -> OLTP vs OLAP
As a RevOps analyst, understanding the differences between OLTP (Online Transaction Processing) and OLAP (Online Analytical Processing) systems can greatly help you in streamlining various operational and analytical tasks. Here's a straightforward explanation aimed at a business user like yourself:

#### OLTP Systems: The Workhorses of Daily Transactions
**What They Do**
OLTP systems are designed to manage and handle everyday business transactions efficiently. These systems are what you interact with when you're doing routine tasks such as entering data, updating records, or processing sales. They are built to be fast and reliable at these types of tasks.

**Characteristics**

**Speed and Efficiency**
OLTP systems are optimized for speed and can handle a large number of transactions by multiple users simultaneously.
**Detailed and Current**
The data in OLTP systems is very detailed, up-to-date, and typically organized at a transactional level (like individual sales or customer interactions).
**Business Use Example**
If you're entering a new customer into a CRM system or processing a sales order, you're likely using an OLTP system. These systems ensure that such operations are performed quickly and accurately.

#### OLAP Systems: The Analysts of Historical Data
**What They Do**
OLAP systems are designed for querying and analyzing historical data. These systems allow you to look at big volumes of data from different angles to understand trends, patterns, and insights. They are not focused on recording transactions but on helping you make sense of what those transactions mean over time.

**Characteristics**

**Complex Queries**
OLAP systems are optimized for complex queries that involve aggregating large amounts of data (like total sales over the last year or comparison of quarterly revenues).
Data Organization: The data in OLAP systems is typically summarized and organized differently from OLTP systems, often in multidimensional structures that make complex queries and report generation easier.
Business Use Example: If you're trying to analyze sales trends over the past five years to predict future demands or to assess the performance of different regions or products, you'd turn to an OLAP system. These systems help you delve into the data to extract strategic insights.

#### Key Differences in Basic Terms
Purpose: OLTP systems are about capturing and storing individual transaction data in real-time. OLAP systems, on the other hand, are about analyzing that data to extract insights and inform decisions.
Data Handling: OLTP systems deal with data at a very granular level, focusing on the accuracy and speed of each transaction. OLAP systems work with aggregated and historical data to help understand broader trends.
Performance: OLTP systems are optimized for a high volume of small, rapid transactions. OLAP systems are optimized for fewer, more complex queries that scan and analyze large datasets.

#### Why This Matters to You as a RevOps Analyst
Understanding these systems can help you better manage the tools and data at your disposal. For instance, knowing when to use OLAP tools can enhance your ability to provide strategic insights for forecasting, planning, and decision-making. Similarly, efficient use of OLTP systems can improve the accuracy and efficiency of day-to-day operations in your role.
By differentiating between these systems, you can more effectively align your technology use with your business objectives, ensuring that both operational efficiency and analytical depth are achieved.

### -> Data Source
From the point of view of a RevOps analyst, the definition of a Data Source in Tinkery, is described as a connection to a specific dataset in a spreadsheet or a group of tables within a database,this  provides an important foundation for both data management and analysis. Let's expand on this concept in terms of its application, management, and strategic significance:

#### Application of Data Sources in RevOps

**Central Access Point**
As a RevOps analyst, you often need a reliable and consistent source of data for operational and analytical purposes. A data source in Tinkery serves as this central access point, where you connect directly to the raw data stored in its original infrastructure (like a cloud database or local server). This means you're working with the most current and comprehensive data available, which is crucial for both accuracy and timeliness in decision-making.

**Integration of Various Data Streams**
In RevOps, you deal with data from multiple aspects of the business, including sales, marketing, customer support, and product usage. Each of these may reside in different spreadsheets or databases. By defining each as a separate data source in Tinkery, you can streamline the process of integrating these varied data streams into a cohesive analysis model. This is essential for providing a 360-degree view of the customer journey and operational efficiency.

**Automation and Reporting**
With direct connections to data sources, you can automate the extraction, transformation, and loading (ETL) processes, thereby saving time and reducing errors. Automated reports can be generated using real-time data, providing ongoing insights into business operations and market conditions.

#### Management of Data Sources

**Data Governance**
Managing data sources effectively involves setting up clear governance around who can access and manipulate the data. This includes defining roles and responsibilities to ensure data integrity and security.

**Data Quality Assurance**
Regular audits and checks are crucial to ensure that the data remains accurate and reliable. As data flows from its source through different analysis tools, maintaining its quality is imperative for making sound business decisions.

**Scalability and Maintenance**
As the business grows, so too will its data needs. Data sources must be scalable and easy to maintain. This might involve upgrading database solutions or migrating data to more robust systems that can handle increased loads and complex queries more efficiently.

#### Strategic Significance of Well-Managed Data Sources

**Enhanced Decision-Making**
With reliable data sources, as a RevOps analyst, you can generate precise and timely insights that drive strategic business decisions. Whether it’s optimizing the sales pipeline, improving customer retention strategies, or adjusting pricing models, accurate data is key.

**Competitive Advantage**
In today’s data-driven world, having direct access to well-organized and manageable data sources provides a competitive edge. It allows for swift adaptation to market changes and more effective targeting and segmentation strategies.

**Operational Efficiency**
Well-defined data sources reduce redundancy, minimize manual data handling, and streamline workflows. This leads to more efficient operations across departments and better allocation of resources.

### -> Data Set

A data set is essentially a collection of data organized in a spreadsheet or a database table. Think of it like a grid, where the vertical columns are known as fields, and the horizontal rows are called records. In Tinkery, both "fields" and "records" are commonly used terms. Sometimes, you might also hear records being called "registries." When you interact with Tinkery, you can use any of these terms. Tinkery's advanced language understanding capabilities ensure that it recognizes and responds correctly to different terminologies you use. This flexibility allows you to communicate naturally without worrying about specific jargon.

### -> Recipes

Think of Recipes within Tinkery as you would any recipe in your kitchen. They consist of carefully crafted instructions designed to help you build projects tailored to your specific needs. Tinkery Recipes will guide you through the setup process, help you understand the type of data required, and even assist you in preparing for your first insights. This step-by-step approach ensures you can start your project confidently and efficiently.

### -> Project

A Project within Tinkery involves a series of datasets that are connected by a common theme or domain. For instance, imagine you are working on a project that requires customer data from your organization's CRM, campaign data from your marketing tool, and conversion data from your organization's database. By creating a Project space in Tinkery, you indicate that the selected datasets are related and will be used to determine specific metrics needed for your project. Tinkery’s AI Engine will then handle the task of building these relationships, assisting you in defining metrics, and even creating visualizations to help you understand the insights you gain from exploring your data.

### -> Ontology

The term "ontology" in the context of a platform like Tinkery typically refers to a formal representation of knowledge as a set of concepts within a domain, and the relationships between those concepts. It's a way to structure and define the data so that it can be easily processed and understood by computer systems. Here’s a breakdown of how ontology might be used in Tinkery, assuming it's a technology-focused platform

#### **Definition and Purpose**

**Conceptual Framework**
An ontology provides a structured framework for organizing information. It defines various categories and concepts within a domain, how these categories interact, and the rules that govern them.

**Common Understanding**
It helps to ensure that there is a common understanding of information that allows diverse systems to interact with each other effectively. This is crucial in environments where integration and interoperability are necessary.

#### **Components of an Ontology**

**Classes**
These are the concepts or categories within the domain. For example, in a business environment, classes could include "Customer", "Order", "Product", etc.

**Attributes**
Characteristics or properties of the classes. For instance, a "Customer" might have attributes like "Name", "Address", and "Phone Number".

**Relationships**
How the classes relate to one another. For example, an "Order" might be related to a "Customer" through a "Placed By" relationship.

**Constraints**
Rules that govern the properties of classes and their relationships. For instance, a constraint might state that every "Order" must have at least one "Product".

#### **Usage in Tinkery**

**Data Modeling**
Ontologies can be used to model data structures on platforms like Tinkery, which would help in organizing data from various sources (e.g., databases, spreadsheets) into a coherent structure.

**Semantic Web and AI**
If Tinkery uses AI and semantic technologies, ontology plays a crucial role in making data machine-readable and understandable by AI algorithms, enhancing capabilities such as machine learning, natural language processing, and decision support systems.

**Integration and Interoperability**
In multi-system environments, ontologies help maintain data consistency and support seamless integration between different systems and components within Tinkery.

#### **Practical Example**

If Tinkery is used to manage enterprise operations, an ontology could define how different aspects of the business are related. It might specify how sales data relates to inventory levels or how customer feedback should be linked to product development processes. This would allow users to perform complex queries across various data sets and generate insights that are relevant and based on a holistic view of the business.


_Last update 8 November 2024_



## Your First Tinkery Project



## Uploading Files



## Connecting Data Sources

## Tinkery AI

## Prompting Guidelines
