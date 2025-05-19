# API Ingestion to a Lakehouse
Lagos Weather API Data Ingestion To Microsoft Fabric Lakehouse from an API source point

🌎 Project Overview




This was a simple ETL ingesting Lagos weather Data from an API source to fabric lakehouse and creating an email notification for the refresh of the ingested data

🤷 What This Project Does





•	Creates a data pipeline




•	Ingests real_time weather data from Open weather API using copy activity in the data pipline


•	Stores and updates data in a Delta table in Microsoft Fabric Lakehouse


•	Transforms and cleanses data using Data flow


•	Stores and updates data in a  table in Microsoft Fabric Warehouse


•	Uses Outlook feature to trigger email alerts for successful run or fail of the pipeline




📆 Tools & Technologies Used








•	Data pipeline



•	Microsoft Fabric Lakehouse 



•	Microsoft Fabric Warehouse



•	Openweather API



•	Data flow



•	Office 365 Outlook (for alerts)



🔧 Steps taken for the project
1. Create a workspace in Microsoft fabric
2. Setup Lakehouse within the created worspace in Fabric

3. Setup Warehouse within the created worspace in Fabric
4. Create a Data pipleine item

  
 • Use copy activity to ingest data from the api source


•	Provide the base Url (api.openweathermap.org)


•	Relative Url fro the lagos weather data(/data/2.5/forecast?lat=6.5244&lon=3.3792&appid={yourAPIKey}


•	Test and preview data


•	Destination will be the lakehouse inputting the new table to be created


   
6. Add data flow item in the pipeline which igestes the new table from the lakehosue to the warehouse
7. Include the outlook activity for both success and fail email notification
8. Validate pipeline
9. Run Pipeline



📷 Screenshot Highlights

![image](https://github.com/user-attachments/assets/64ceb532-4284-4d35-b20b-d8d7459b7f55)




Table ingested to the lakehouse


![image](https://github.com/user-attachments/assets/ec9e48bb-a44a-4222-8fa4-c1e2834e6586)




Table Ingested to the Warehouse


![image](https://github.com/user-attachments/assets/3ba50e5e-e042-461d-8879-89f22127f4d0)



Email Notification


![image](https://github.com/user-attachments/assets/a2e3e994-9486-4ac3-8cee-88f12025e890)


🧡 Importance



This project uses  low-code tools and cloud-native orchestration . It shows how Microsoft Fabric can be used to automate ingestion, transform and create alerts in a unified platform.



📆 Author

Adebola Okunlade


Data Engineer | Analytical Engineer |Microsoft Azure and Fabric Engineer 



Want to collaborate or connect? www.linkedin.com/in/adebola-okunlade












