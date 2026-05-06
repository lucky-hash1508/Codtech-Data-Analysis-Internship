#CODTECH DATA ANALYSIS INTERNSHIP#-
All 4 internship tasks submission

*COMPANY*: CODTECH IT SOLUTION

*NAME*: ASMIT ARVIND SHAH

*INTERN ID*: CTIS7975

*DOMAIN*: DATA ANALYTICS

*DURATION*: 6 WEEKS

*MENTOR*: NEELA SANTOSH
_______________________________________________________________________________________________________________________________________________________________
1) **TASK1- BIG DATA ANALYSIS:**

##DESCRIPTION OF THE TASK-

In this task, I performed big data analysis using PySpark, which is a powerful tool used for processing large datasets efficiently. The main objective of this task was to understand how big data tools work and how they can be used to analyze data at scale. For this purpose, I used Google Colab as my working environment and installed PySpark to create a Spark session. This session allowed me to handle data in a distributed manner, which is one of the key advantages of using PySpark over traditional data processing tools. I worked on a dataset related to restaurant tips, which includes details such as total bill, tip amount, gender, day, and other attributes. Initially, I faced an issue while directly loading the dataset using a URL, but I resolved it by first loading the data using Pandas and then converting it into a format readable by PySpark. This helped me understand practical challenges and how to solve them during real-world data analysis tasks.

After successfully loading the dataset into a PySpark DataFrame, I started by exploring its structure using the printSchema() function. This step was important because it helped me understand the data types of each column, such as numerical and categorical variables. Then, I performed basic analysis by counting the total number of records in the dataset, which gave me an idea about the size of the data. I also calculated the average value of the total bill using aggregation functions, which is a common operation in data analysis. These initial steps helped me build a foundation for further analysis. I made sure to follow proper syntax and functions in PySpark, and I learned how similar operations are performed differently compared to normal Python libraries like Pandas.

Further, I performed grouping operations to extract meaningful insights from the dataset. I grouped the data based on gender to analyze differences in spending behavior, and also grouped it by the day of the week to understand how customer spending varies across different days. From the results, I observed that weekends like Sunday and Saturday have higher average total bills compared to weekdays, indicating higher customer activity. I also performed tip analysis to see how tipping behavior changes based on the day. These insights are useful in real-world scenarios, especially for businesses to make decisions based on customer patterns. Overall, this task helped me understand the practical implementation of big data analysis using PySpark and improved my skills in handling datasets efficiently while extracting meaningful information.

#OUTPUT-

<img width="494" height="554" alt="Image" src="https://github.com/user-attachments/assets/13f7838a-9bad-4aba-a8c0-bbdbc0d7d9a6" />

____________________________________________________________________________________________________________________________________________________________________
2) **TASK2- PREDICTIVE ANALYSIS USING MACHINE LEARNING:**
##DESCRIPTION OF THE TASK-

In this task, I performed predictive analysis using machine learning techniques with the help of PySpark in a Google Colab environment. The primary objective was to build a regression model that could predict the tip amount based on the total bill using a real-world dataset. To begin with, I set up the environment by installing PySpark and initializing a Spark session, which is essential for handling large-scale data processing. The dataset used for this task was the popular “tips” dataset, which contains information about restaurant bills, including attributes such as total bill amount, tip, gender, smoking status, day, time, and size of the group. Since PySpark does not directly support loading data from an online URL, I first downloaded the dataset using the Pandas library and then saved it locally as a CSV file. After that, I loaded the dataset into a PySpark DataFrame with schema inference enabled, allowing the system to automatically detect the correct data types of each column.

After successfully loading the dataset, I moved on to preparing the data for machine learning. In PySpark, machine learning models require input features to be in vector format, so I used the VectorAssembler tool to convert the selected feature into the required format. In this case, I selected the “total_bill” column as the input feature and the “tip” column as the target variable. The assembler transformed the dataset by creating a new column called “features,” which contained the input values in vector form. This step is crucial because machine learning models in PySpark cannot directly work with raw columns. Once the data preparation was completed, I implemented a Linear Regression model, which is a widely used algorithm for predicting continuous numerical values. The model was configured by specifying the feature column and label column, and then it was trained using the prepared dataset. During this process, the model learned the relationship between the total bill and the tip amount.

Finally, I evaluated the performance of the model by generating predictions and analyzing the results. Using the trained model, I applied the transform() function to produce a new DataFrame that included a “prediction” column along with the original values. This allowed me to compare the actual tip values with the predicted ones, giving a clear understanding of how well the model performs. The results showed that the predicted values were quite close to the actual values, indicating that the model was able to capture the relationship between the variables effectively. Additionally, I examined the model’s coefficients and intercept, which provided further insight into how the model makes predictions. The coefficient indicated a positive relationship between the total bill and the tip, meaning that as the bill increases, the tip also tends to increase. Overall, this task helped me understand the complete workflow of building a machine learning model using PySpark, including data loading, feature engineering, model training, prediction, and evaluation, and demonstrated how predictive analysis can be used to derive meaningful insights from data.

#OUTPUT-

<img width="397" height="556" alt="Image" src="https://github.com/user-attachments/assets/8e944ce3-783b-4239-87ea-c26ef25e1aa6" />

_______________________________________________________________________________________________________________________________________________________________
3) **TASK3- DASHBOARD DEVELOPMENT:**

##DESCRIPTION OF THE TASK-

In this task, I developed an interactive dashboard using Power BI to visualize and analyze a dataset effectively. The primary objective of this task was to transform raw data into meaningful visual insights that can support decision-making. The dataset used for this project was the “tips” dataset, which contains information about restaurant transactions, including total bill amount, tip, gender, smoking status, day, time, and group size. Initially, I loaded the dataset into Power BI by importing the CSV file using the “Get Data” feature. Once the data was successfully loaded, I explored the dataset to understand the available fields and ensure that the data types were correctly assigned.

After loading the dataset, I proceeded to create various visualizations to represent the data in an interactive and understandable format. The first visualization created was a bar chart that displayed the average total bill amount for each day of the week. This chart provided insights into customer spending patterns, showing that weekends, especially Sunday and Saturday, had higher average bill amounts compared to weekdays. This indicates that customer activity and spending are higher during weekends. The second visualization was a pie chart that illustrated the distribution of customers based on gender. The chart revealed that a higher percentage of customers were male compared to female, which provides useful information about customer demographics.

In addition to these visualizations, I created a line chart to analyze the trend of tip amounts across different days of the week. This chart helped in understanding tipping behavior and identifying patterns over time. It showed that tips tend to be higher on weekends, which aligns with the observation of higher total bill amounts during those days. This indicates a positive relationship between customer spending and tipping behavior. Finally, I arranged all the visualizations in a structured layout and added a title to create a complete and professional dashboard. The dashboard provides actionable insights such as peak business days, customer demographics, and tipping trends. Overall, this task demonstrates the importance of data visualization in data analysis and highlights how Power BI can be used to create interactive dashboards that simplify complex data into meaningful insights.

#OUTPUT-

<img width="1312" height="736" alt="Image" src="https://github.com/user-attachments/assets/49bc2250-3e8a-48e1-9400-7c0b11d6a592" />

_______________________________________________________________________________________________________________________________________________________________
4) **TASK4- SENTIMENT ANALYSIS:**

##DESCRIPTION OF THE TASK-

In this task, I performed sentiment analysis on textual data using Natural Language Processing (NLP) techniques in a Python-based environment. The main objective of this task was to analyze text data and determine whether the sentiment expressed in each text is positive, negative, or neutral. Sentiment analysis is a widely used NLP technique that helps in understanding opinions, emotions, and attitudes from textual information such as reviews, feedback, or social media posts. To implement this, I used the TextBlob library, which is a simple and effective NLP tool for processing textual data and performing sentiment analysis. Initially, I installed the required library and imported necessary modules such as pandas for handling data and TextBlob for analyzing text. A dataset was then created consisting of multiple text reviews representing different types of sentiments.

After preparing the dataset, I moved on to the data preprocessing and model implementation phase. The textual data was structured into a pandas DataFrame for easy manipulation and analysis. A custom function was defined to evaluate the sentiment of each review using TextBlob. This function calculated the polarity score of the text, which ranges from -1 to +1. Based on this score, each review was classified into three categories: positive, negative, or neutral. Reviews with a polarity greater than zero were labeled as positive, those with a polarity less than zero were labeled as negative, and those with zero polarity were considered neutral. This step represents the implementation of the sentiment analysis model, where the algorithm processes each piece of text and assigns a sentiment label. The function was then applied to the entire dataset using the apply() method, resulting in a new column that displayed the sentiment classification for each review.

Finally, I analyzed the results and generated insights from the sentiment analysis. The output displayed both the original reviews and their corresponding sentiment labels, providing a clear understanding of how each text was interpreted by the model. Additionally, I calculated the count of each sentiment category using value_counts(), which helped summarize the overall sentiment distribution in the dataset. A bar chart was also created to visually represent this distribution, making it easier to interpret the results. The analysis revealed that the dataset contained an equal number of positive and negative sentiments, indicating a balanced set of opinions. This task demonstrates how NLP techniques can be used to extract meaningful insights from textual data and highlights the importance of sentiment analysis in real-world applications such as customer feedback analysis, product reviews, and social media monitoring. Overall, this task provided practical experience in handling text data, applying NLP techniques, and generating actionable insights through sentiment classification.


#OUTPUT-


<img width="237" height="209" alt="Image" src="https://github.com/user-attachments/assets/147f5731-7334-491a-a398-99ed9c95ec81" /> 

<img width="708" height="628" alt="Image" src="https://github.com/user-attachments/assets/ffa97255-533d-4d62-a681-f1aeb25aab97" />

