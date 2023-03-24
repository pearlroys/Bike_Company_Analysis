# bike_company-analysis
# The Tools 
    - Python, SQL, 
    Tableau (Tableau Public since I don’t currently have a Tableau Desktop subscription), 
    Kaggle to source data
- The Steps 
    - Source data (CSVs from Kaggle)
    - Create a BigQuery dataset and associated tables
    - Query data using Python
    - Push finalized CSV to Google Drive
    - Connect to cleaned CSVs using Tableau Public
    - Analysis
    - Visualization

# TASK
- As a junior data analyst in Cyclistic's marketing team, your task is to assist in devising marketing strategies that target casual riders with the aim of converting them into annual members. The marketing director believes that the company's success in the future hinges on maximizing the number of annual memberships. 
- However, before presenting their recommendations, Cyclistic's executives require compelling data insights and professional data visualizations to back up the proposed strategies.
- The team's objective is to analyze Cyclistic's historical bike trip data to identify trends that will shed light on the differences between casual riders and annual members, why casual riders would be interested in purchasing a membership, and how digital media could impact the effectiveness of their marketing tactics.
## ASK PHASE:
    I carefully reviewed and analyzed the needs and expectations of the stakeholders,  i then dived into the exciting task at hand! We need to uncover patterns within the data that will allow us to distinguish between casual riders and members. 
    By gaining a deeper understanding of our users' behavior, we can provide the marketing team with valuable insights that will help them create more effective strategies. This is an opportunity for us to explore and uncover new, game-changing discoveries that will help drive the success of our business. Let's get started!
    
## PREPARE:
    The data is provided to us as CSV files, with each file containing data for a single month.
    The case study's dataset was downloaded , I had to download information from the previous 12 months. I downloaded trip information from December 2021 to December 2022. The datasets are available here. It is a public dataset that Motivate International Inc. has made available.
    The data was inspected and I tried to make sense of the different fields and rows using excel.
    
## PROCESS:
 Now, brace yourself for a thrilling data adventure! To streamline our analysis, I combined multiple files and read it using Pandas. After scrubbing the data to remove duplicates, deleting rows with invalid ride start and end times, adding more columns such month, day of the week and time used . I proceeded to query the data with SQL.
    
    - 
<img width="593" alt="Screenshot 2023-03-24 at 07 27 08" src="https://user-images.githubusercontent.com/103274172/227455458-0688998e-7549-4212-9c98-fda651bf5425.png">
    - While Pandas is a popular option, using SQL Is the go-to language for querying and manipulating data. In the code I provided, I used SQL Lite. However, in my other projects I'd ideally use  a cloud-based storage service like GCP, AWS, or Azure to store and query the data. The end result? A pristine dataset that's ready to reveal its secrets and help us make informed business decisions. 
    <img width="914" alt="Screenshot 2023-03-24 at 07 28 14" src="https://user-images.githubusercontent.com/103274172/227455555-2a3767ad-7bd4-41f8-946e-4370d6ff5e73.png">
- 
## ANALYZE:
- When you first encounter a new dataset, it's important to approach it with an open mind and a sense of curiosity. Resist the temptation to dive too deep into insights right away. Instead, start by exploring the data and writing queries that you think will yield interesting results. Allow yourself to play and experiment with different approaches, and don't be afraid to follow unexpected paths. Who knows what hidden gems you might uncover? To help you get started, here are some starter queries I used to get 'friendly' with my dataset 😂 .
- <img width="717" alt="Screenshot 2023-03-24 at 07 29 04" src="https://user-images.githubusercontent.com/103274172/227454913-30853fcb-02b1-493e-bd66-4923cb4263ab.png">
- 
<img width="432" alt="Screenshot 2023-03-24 at 07 29 22" src="https://user-images.githubusercontent.com/103274172/227455029-28076fbf-d668-408f-a283-f67245684997.png">
- <img width="481" alt="Screenshot 2023-03-23 at 17 19 23" src="https://user-images.githubusercontent.com/103274172/227454761-40e38233-7b69-4020-bdc2-4bd93b64693c.png">

- Once you feel like you have 3–5 compelling insights, you have enough to populate a dashboard without cluttering it.
- SHARE
    - I created more data visualizations in Tableau. I then combined the visualizations on a dashboard that can be viewed here. 
    
# RECOMMENDATIONS
- I'd want to present my hypothesis on this topic based on the results of my analysis and to wrap up my observations.
    - I strongly believe that the casual members are mainly composed of tourists and or families who wish to spend their trips and or weekends sightseeing as well as carrying out leisure activities. This can be confirmed by the most frequented locations by casual users
    - <img width="393" alt="Screenshot 2023-03-24 at 07 33 33" src="https://user-images.githubusercontent.com/103274172/227455091-21a4dec6-20da-43ac-89e1-57740a58007b.png">
    - There is a strong predisposition to believe that the majority of our annual members are employed individuals who utilise our services as their primary mode of transportation which can be seen on the map also.
    - <img width="588" alt="Screenshot 2023-03-24 at 07 32 41" src="https://user-images.githubusercontent.com/103274172/227455215-6d68c20a-c7f8-472f-9df7-6050fcee4f78.png">
    - To attract casual riders, emphasise the advantages of membership, such as discounts and privileges.
    - Encourage current users to utilise a hashtag on social media to express their own experiences with Cyclistic and how it has impacted their life in order to foster a feeling of community.

### Now, to answer Moreno’s and her team’s request, which was: To design marketing strategies to convert casual riders into annual members. I would suggest the following:
    - We can clearly see a peak in casual riders on a few occasions: On the weekends as well as in the months of June, July & August. we should prioritize marketing during these periods.
    - As a follow up to the previous suggestions, we should advertise promotions during these months to allow casual members upgrade to annual members at a discount.
    - I would suggest strategically enforcing location-based advertisements (featured on Instagram & Facebook) to target the top 10 popular stations among the casual members.
    - Increasing the pricing of single-day & full-day passes while simultaneously emphasising the appeal of membership. By strategically pricing it higher, it would appeal to upgrade to an annual membership.
- 
### Additional remarks:
- It would be great if I had a dataset that did not format single-ride passes and full-day passes into ‘casual’ in the member types as we would be able to more intricately analyze the data regarding trip durations and make more specific recommendations
- Unique user IDs would allow me to count how many times an individual has used the service which would allow for more intricate and strategic promotions
- Casual riders tend to make the most of their trips on Wednesdays and Thursdays. 
