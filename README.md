# Stocker – Cloud Based Stock Trading Application

Stocker is a **cloud-based stock trading web application** built using the **Flask framework** and **AWS cloud services** such as DynamoDB, SNS, and EC2.  
It allows users to **register, login, view available stocks, buy/sell stocks, and manage their portfolio** with real-time cloud database updates and notifications.

---

## Features

- User Registration and Login
- Trader Dashboard
- Admin Dashboard
- View Available Stocks
- Buy Stocks
- Sell Stocks
- Portfolio Management
- Real-time Database Updates
- Email Notifications using AWS SNS
- Cloud Deployment using AWS EC2

---

## Technologies Used

### Backend
- Python
- Flask

### Frontend
- HTML
- CSS
- Jinja2 Templates

### Cloud Services
- AWS DynamoDB (Database)
- AWS SNS (Notifications)
- AWS EC2 (Deployment)

### Libraries
- boto3
- Flask
- python-dotenv

---

## Project Architecture


User Browser
↓
Flask Web Application (EC2)
↓
AWS DynamoDB Database
↓
Amazon SNS Notification System


---

## DynamoDB Tables

The application uses four DynamoDB tables:

| Table | Description |
|------|-------------|
| Users | Stores user account details |
| Stocks | Stores available stock information |
| Transactions | Stores buy/sell records |
| Portfolio | Stores user stock holdings |

---

## Application Pages

- Home Page
- Signup Page
- Login Page
- Trader Dashboard
- Admin Dashboard
- Portfolio Page

---

## Example Stocks

| Stock | Symbol | Price |
|------|------|------|
| Apple | AAPL | $180 |
| Tesla | TSLA | $240 |
| Google | GOOG | $130 |

---

## Installation

Clone the repository:


git clone https://github.com/nithin-t-bot/stocker.git


Navigate to project folder:


cd stocker


Install dependencies:


pip install -r requirements.txt


Run the application:


python app.py


Open browser:


http://localhost:5000


---

## Deployment

The application can be deployed on **AWS EC2**.

Steps:

1. Launch EC2 instance
2. Install Python and Git


sudo yum update -y
sudo yum install python3 python3-pip git -y


3. Clone the repository


git clone https://github.com/nithin-t-bot/stocker.git


4. Install requirements


pip3 install -r requirements.txt


5. Run application


python3 app.py


6. Open website


http://EC2_PUBLIC_IP:5000


---

## Conclusion

This project demonstrates how **Flask web development can be integrated with AWS cloud services** to build a scalable stock trading platform. DynamoDB provides efficient database storage while SNS enables real-time notifications, making the system reliable and cloud-ready.

---

## Author

**Nithin T**  
Cloud Computing Project  
BIET
