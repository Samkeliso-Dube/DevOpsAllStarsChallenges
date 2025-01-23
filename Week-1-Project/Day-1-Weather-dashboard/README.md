# Weather Dashboard Project

This project is **Day 1/30** of the **DevOps Challenge** and focuses on creating a weather dashboard. The dashboard collects real-time weather data from a Weather App API and stores it in an AWS S3 bucket for further use and analysis.

---

## **Objectives**
- Fetch real-time weather data for a specified city.
- Save weather data as JSON files.
- Upload the JSON files to an AWS S3 bucket.

---

## **Tools**
- **Programming Language**: Python  
- **Cloud Service**: AWS S3  
- **Weather API**: OpenWeatherMap or any suitable weather API  
- **Libraries**:
  - `requests`: To make API calls  
  - `boto3`: To interact with AWS S3  

---

## **Project Structure**
```
weather-dashboard/
  src/
    __init__.py
    weather_dashboard.py
  tests/
  data/
  .env
  .gitignore
  requirements.txt
```


---



---

### **Getting Started**
1. Clone this repository:
   ```bash
   git clone https://github.com/ShaeInTheCloud/30days-weather-dashboard.git

   cd weather-dashboard
   ```

2.Install the required libraries:
```
pip install -r requirements.txt
```
## **AWS S3 Bucket**
- Log in to the AWS Management Console.

- Create an S3 bucket (e.g., weather-dashboard-demo).

- Note down the bucket name for use in the script in the **.env** file.

## **Configure AWS Credentials**
Using AWS CLI configure your AWS credentials
```
aws configure
```
You will be prompted to enter the following information:

```
AWS_ACCESS_KEY_ID="******************"
AWS_SECRET_ACCESS_KEY="**************"
AWS_DEFAULT_REGION="*****************"
```

## **Set Up Environment Variables**
Inside the **.env** file in the project directory.
Add the following variables:
```
OPENWEATHER_API_KEY= your_openweather_api_key
AWS_BUCKET_NAME=your_s3_bucket_name
```
You can obtain the OPENWEATHER_API_KEY by signing up for a free account at [OpenWeatherMap](https://home.openweathermap.org/).
## **Run the script**
```
python weather_dashboard.py
```
## **Expected Output**
When the command is successful, you should see output similar to this:
```
Fetching weather data for [City Name]...
Weather data fetched successfully.
Uploading data to AWS S3...
Data uploaded successfully to bucket [your_s3_bucket_name].
```

## **Contribute**
If you want to contribute to this project, feel free to fork the repository, make your changes, and submit a pull request. Contributions are welcome, whether it's improving documentation, adding features, or fixing bugs!
