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

**1) WebScrapping -** The data is extracted from Instahyre(A Job Portal) using Selenium.
   
![258516492-df483f7a-7463-4ad8-a71a-7e1c32b976eb](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/8ccd4e95-df94-4e51-abae-5efc8a443f36)

![258516878-1717a6a6-8d9e-489b-bb50-4dbcf2777d1b](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/d87055cc-87f6-434e-bf43-f95468932cce)

![258517086-d3001359-153b-4f7c-bee8-e34b15ac6f3d](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/26800395-8af7-4f5f-8f91-1d546bcab841)

![258517176-051fde6f-440f-4d47-8a82-ff1f1aadd652](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/eb2aafa9-e9a9-47e1-ac73-1e6a68ad302a)

**2) Data Cleaning -** After getting the Raw data it is cleaned using pandas and numpy in Python. 

**a) Import necessary modules and packages.**

![data_cleaning_1](https://github.com/tuneerdutta/Job-Recomendation-Model/assets/131517578/d027cc80-849f-406d-98da-8d1e97e8c02d)






**----Challenges Faced----**

**1) Model Selection and Tuning:** Choosing the appropriate ML algorithms and hyperparameter tuning can significantly impact the project's success. It might involve experimenting with different models to find the best fit for the recommendation system.

**2) Scalability:** As the amount of scraped data grows, the ML models and infrastructure should be able to handle the increasing scale and provide real-time or near-real-time recommendations.

**3) Team Problem -** As all of our team members are working professionals, we were finding difficulty in managing time and the time availability of each team member is different. Firstly, we brainstormed and formed a flowchart of works that helped us be on track. We allocated the work according to each person’s time availability and task priority

Overall this project can be used to help job seekers identify suitable job opportunities based on their skills. This can save job seekers time and effort in their job search and increase the chances of them finding a job that matches their Skills. This project can have a positive social impact by helping job seekers from diverse background, find meaningful employment opportunities and reducing unemployment rates.




