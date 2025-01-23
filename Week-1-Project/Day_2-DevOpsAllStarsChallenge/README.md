# NBA Game Updates  

Welcome to the **NBA Game Updates ** project! 🎉 This application is designed to deliver real-time NBA game updates to subscribers using AWS services.  

## Project Overview  
This project leverages **AWS SNS**, **Lambda**, **EventBridge**, and the **SportsIO API** to automate the retrieval and delivery of NBA game updates.  

## Features  
- Real-time NBA game updates.  
- Notifications via email, SMS, or other subscribed endpoints.  
- Automated daily updates using AWS EventBridge.  
- Secure and scalable serverless architecture.  

## Architecture  
1. **AWS SNS**: Used as the central notification hub.  
2. **AWS Lambda**: Fetches NBA game data from the SportsIO API and publishes updates to SNS.  
3. **SportsIO API**: Provides real-time NBA game updates.  
4. **AWS EventBridge**: Schedules the Lambda function to run daily.  
5. **IAM Roles & Policies**: Secures access to AWS resources.  

## Setup Instructions  

### Prerequisites  
- AWS Account  
- SportsIO API Key  
- Python 3.9 

### Steps to Set Up  
1. **Create an SNS Topic**:  
   - Go to AWS SNS and create a new topic for notifications.  
   - Add subscriptions (email, SMS, or Lambda).  

2. **Set Up Lambda Function**:  
   - Create a Lambda function in the AWS Console.  
   - Write a Python script to fetch NBA data using the SportsIO API and publish it to SNS.  
   - Add environment variables to store the SportsIO API key.  

3. **Configure IAM Roles and Policies**:  
   - Attach the necessary permissions (e.g., AWSLambdaBasicExecutionRole, SNSFullAccess).  

4. **Integrate with SportsIO API**:  
   - Use the SportsIO API to fetch game data in the Lambda function.  

5. **Automate with EventBridge**:  
   - Schedule the Lambda function to run daily using EventBridge.  

## Technologies Used  
- **AWS SNS**  
- **AWS Lambda**  
- **AWS EventBridge**  
- **Python**  
- **SportsIO API**  

## Contributing  
Feel free to contribute by opening issues or submitting pull requests. Let’s build this project together!  

## Contact  
For questions or feedback, connect with me on [LinkedIn](www.linkedin.com/in/samkeliso-dube).  

---

Let me know if you'd like any modifications or additional details! 🚀  
