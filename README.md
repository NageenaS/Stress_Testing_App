# Stress_Testing_App

The Stress Testing App is a powerful tool designed to evaluate and monitor the performance of various system resources, including memory, disk, CPU, network, and MySQL databases. 

# Features
-- Memory Stress Testing: Allocates memory and monitors its usage to assess stability.
-- Disk Performance Testing: Writes large files to measure disk I/O capabilities.
-- Network Stress Testing: Simulates heavy network traffic to evaluate bandwidth usage.
-- CPU Stress Testing: Performs intensive calculations to gauge CPU performance.
-- MySQL Database Testing: Executes SQL queries to analyze database load handling.
-- AI-Driven Logging: Utilizes AI to provide insights on performance metrics.
-- WhatsApp Notifications: Sends real-time alerts and suggestions through WhatsApp.

# Installation
Clone the Repository:

To get started, clone the repository to your local machine:
```
git clone https://github.com/NageenaS/Stress_Testing_App.git
cd Stress_Testing_App
```
Install Dependencies:

Make sure to install the required Python libraries:
```
pip install psutil mysql-connector-python
pip install twilio
```
Deploy with Docker :

You can quickly deploy the application using Docker. Follow these steps:

Pull the pre-built image:

```
docker pull nageenashaik/stress_testing_app
```
Start the container:
```
docker run -d --name stress_tester nageenashaik/stress_testing_app
```
Executing Stress Tests
To begin your stress testing, run the following command:
```
python app.py
```
If you're running it in a Docker container:
```
docker exec -it stress_tester python app.py
```

# Logging and Alerts
The application generates detailed logs of each test in stress_test.log. Additionally, you can enable WhatsApp notifications by configuring the send_to_whatsapp.py script with your Twilio account details.

# Continuous Integration
This project includes a Jenkinsfile to automate CI/CD processes, ensuring that every update is tested and deployed efficiently.

