# Job-Recommendation-Model

![Screenshot 2023-08-05 085842](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/299d06cb-3d80-4bc3-bfd1-b445967db13b)

**----Introduction----**

Instahyre is an advanced hiring platform based on artificial intelligence, enabling recruiters to hire top talent effortlessly.
Trusted by 10,000+ companies including Google, Amazon, Flipkart, Microsoft, Uber, Walmart, Swiggy, and more!

**----Problem Statement----**

To help Job seekers and career professionals with the information they need to make informed decisions about their careers.
To Develop an user-friendly application to find relevant job opportunities and gain insights based on their skill set. 

**----Objectives----**

Develop an application that provides useful insights and relevant job openings based on skills. The goal is to help job seekers and professionals to gain a better understanding of job market, including the most common location, experience level, relevant class, and total number of jobs available. The application should be scalable and should be able to accommodate the addition of new features in the future.

**----Data Description----**

**1) Excel_Files -** This folder contains the final clean data which was cleaned using numpy as pandas after extracting from the website Instahyre through WebScrapping. Also it contains the Pivot Table Insights which was visualized from the above scrapped data.

**2) Python_Jupyter_Notebook -** This folder contains all the WebScrapping related python files. It contains the DataCleaning Jupyter Notebook file  followed by the Linkedin.py file which contains the data about the Linkedin Followers Count. Then the Spell Checkers file which is used to correct the spelling while we search for a particular skill. Is also contains the app.py file which contains the HTML and Python combine code for the Streamlit app on which the model is deployed.

**3) App Link -** This folder contains the link of the Job Recommendation App.

**4) Power Point Presentation -** This folder contains the PPT for visualizing and analysing the whole Project.


**----Project Overview----**

**1) WebScrapping :-** The data is extracted from Instahyre(A Job Portal) using Selenium.
   
![258516492-df483f7a-7463-4ad8-a71a-7e1c32b976eb](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/8ccd4e95-df94-4e51-abae-5efc8a443f36)

![258516878-1717a6a6-8d9e-489b-bb50-4dbcf2777d1b](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/d87055cc-87f6-434e-bf43-f95468932cce)

![258517086-d3001359-153b-4f7c-bee8-e34b15ac6f3d](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/26800395-8af7-4f5f-8f91-1d546bcab841)

![258517176-051fde6f-440f-4d47-8a82-ff1f1aadd652](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/eb2aafa9-e9a9-47e1-ac73-1e6a68ad302a)

**2) Data Cleaning :-** After getting the Raw data it is cleaned using pandas and numpy in Python. 

**a) Import necessary modules and packages -**

![data_cleaning_1](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/d027cc80-849f-406d-98da-8d1e97e8c02d)

**b) Cleaning the Skills & Location Columns -** The skills column is splitted into number of skills the particular cell has.

![data_cleaning_2](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/be359bdf-4f50-4804-8f19-20162b0dcf51)

![data_cleaning_3](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/f25d4302-a9f0-416f-a7d8-941cc8336805)

**c) Splitting the Employees Count Column with the help of a Delimiter -** 

![data_cleaning_4](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/211b8514-0b8f-4535-8629-4b92429b14ad)


**d) Scalling the Numerical Columns -** All the numerical columns are scaled using the StandardScaler Class. 

![data_cleaning_5](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/1b9e61e7-339e-4cbb-8092-a58b7646c4b0)


**3) Creation of the ML clustering Model using KMeans :-** KMeans performs partition-based clustering by grouping data points into 'k' clusters, where 'k' is a user-defined hyperparameter. The model is built using the Employees count and the Followers in a particular job which predicts the Class to which the particular job belongs.

![kmeans_1](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/2ca4d2a2-b0ff-4711-91da-30958bd5fcd8)

![kmeans_2](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/d74b32b8-d1d8-41b5-9ae6-61d57dc5ce67)

**4) Scatter Plot to visualize the Employees Count with the Followers with Clusters determined by the Color :-**

(Cluster 0 - Green
Cluster 1 - Red
Cluster 2 - Black
Cluster 3 - Blue)

![download](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/c683b566-b4f8-40ba-933c-e128b5fa2b00)


**5) Plot the Elbow Graph :-** Visualize the relationship between the number of clusters (k) and the corresponding cost function, typically the sum of squared distances from each point to its assigned cluster center. The elbow graph helps us identify the optimal number of clusters by looking for the "elbow point," where the cost starts to decrease more slowly, suggesting diminishing returns on adding more clusters.

![download](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/e1d2b173-00b4-49f9-9f59-f43336fb2083)

**6) Save the updated DataFrame to a new CSV file :-**  

![kmeans_3](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/789e25aa-12bc-4e00-a307-12101ef9b3b0)

**Job Analytics Recommendation App :-** 

**a) HTML and Python code -** Streamlit is an open-source app framework in python language. It helps us create beautiful web apps for data science and machine learning in a little time. It is compatible with major python libraries such as scikit-learn, keras, PyTorch, latex, numpy, pandas, matplotlib, etc. So this code is for deployment of the model into Streamlit app.

![html_1](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/22e377cd-b12e-44a7-b6e8-f4a49b108f71)

![html_2](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/d7aea71c-d81d-41cd-b0ae-f4ffcf4fbe6f)

![html_3](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/d43d1eeb-c341-4d74-8265-59d8c903da0b)

**Job Analytics Recommendation App :-**

This app is made with HTML and Python to deploy the clustering ML model which predits the Most Common Experience Level, Most Common Workplace, Most Common Class, Total Number of Jobs Avalilable according to skills provided in the searck box. The skills are independent on the spellings of the Skills. After that we can see the job details of those specific jobs and we can also apply into those jobs according toi our needs.

![app](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/6abf97a1-a73d-498a-b697-99201a333670)

![app_1](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/36df681c-4e2b-405b-a4de-819f8c149b88)

![app_2](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/976af744-15c9-4aa6-92f1-04ac58663afa)


**----Insights----**

**1) Most of the listed companies on Instahyre have low LinkedIn Followers.**

![insights_1](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/22137eed-b8b5-4efc-a42f-5d3bb9b0c4ab)


**2) Companies Founded after year 2000 have the most Job Opportunities.**

![insights_2](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/5d421686-b996-4bf9-8b5a-5a42c9fb6c1d)


3) IT Jobs are high in demand. Software Engineer is the most demanding designation in the market.

![insights_3](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/f169e33c-9ca0-40b5-9ed3-6a22afea4cb9)


4) Job opportunities are higher for experienced candidates as compared to entry-level freshers.

![insights_4](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/ed0fdc61-51fb-4eb8-a7cd-c3d9646ea90f)


**----Conclusion----**

The project successfully provides insights into the job market for popular skills like Python and SQL, which can be valuable for job seekers, employers and industry analysts alike. The analysis of the most common location, experience level, and job classes can be used by job seekers to target their job search and improve their chances of finding a relevant job. Similarly, employers can use this information to refine their hiring strategies and tailor job requirements to the current job market.


**----Challenges Faced----**

a) Scraping LinkedIn followers of different companies without getting banned was a challenging task.

b) Proper integration of SpellChecker consumed a lot of time.

c) After ML model deployment, It took us some time and efforts to get familiar with HTML and CSS language for designing UI.


Overall this project can be used to help job seekers identify suitable job opportunities based on their skills. This can save job seekers time and effort in their job search and increase the chances of them finding a job that matches their Skills. This project can have a positive social impact by helping job seekers from diverse background, find meaningful employment opportunities and reducing unemployment rates.




