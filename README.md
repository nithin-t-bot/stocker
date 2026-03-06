# stocker
Stocker is a cloud-based stock trading web application built using Flask and AWS services such as DynamoDB, SNS, and EC2. It allows users to register, login, view available stocks, buy/sell stocks, and manage their portfolio with real-time cloud database updates and notifications.

# Stocker – Cloud Based Stock Trading Application
Stocker is a cloud-based stock trading web application developed using the Flask framework and AWS cloud services. The application allows users to register, log in, view available stocks, buy or sell stocks, and manage their personal trading portfolio. The system uses AWS DynamoDB for storing user accounts, stock details, transactions, and portfolio data.

The application also integrates Amazon SNS (Simple Notification Service) to send notifications whenever a user registers, logs in, or performs stock transactions such as buying or selling stocks.

The project demonstrates how modern cloud services can be used to build scalable and efficient web applications.

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
- SNS Email Notifications
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

- **Users** – Stores user account details
- **Stocks** – Stores available stock information
- **Transactions** – Stores buy/sell records
- **Portfolio** – Stores user stock holdings

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

## Deployment

The application can be deployed on AWS EC2 by installing Python, Flask, and cloning the repository.

Run:

```bash
pip install -r requirements.txt
python app.py
