Stocker – Cloud Based Stock Trading Application

Stocker is a cloud-based stock trading web application built using the Flask framework and AWS cloud services. The application allows users to register, log in, view available stocks, buy or sell stocks, and manage their trading portfolio.

The system uses AWS DynamoDB for storing user accounts, stock details, transactions, and portfolio data. It also integrates Amazon SNS (Simple Notification Service) to send notifications whenever users perform actions such as signing up, logging in, buying, or selling stocks.

This project demonstrates how modern cloud services and web technologies can be combined to build scalable, efficient, and real-time applications.

Features

User Registration and Login

Trader Dashboard

Admin Dashboard

View Available Stocks

Buy Stocks

Sell Stocks

Portfolio Management

Real-time Database Updates

Email Notifications using AWS SNS

Cloud Deployment using AWS EC2

Technologies Used
Backend

Python

Flask

Frontend

HTML

CSS

Jinja2 Templates

Cloud Services

AWS DynamoDB – Database storage

AWS SNS – Email notifications

AWS EC2 – Cloud deployment

Libraries

boto3

Flask

python-dotenv

Project Architecture
User Browser
     ↓
Flask Web Application (EC2)
     ↓
AWS DynamoDB Database
     ↓
Amazon SNS Notification System
DynamoDB Tables

The application uses four DynamoDB tables.

Users

Stores user account details.

Field	Description
user_id	Unique user ID
email	User email
password	User password
role	admin / trader
is_active	Account status
Stocks

Stores available stock information.

Field	Description
stock_id	Unique stock ID
symbol	Stock symbol
price	Stock price

Example stocks:

Stock	Symbol	Price
Apple	AAPL	$180
Tesla	TSLA	$240
Google	GOOG	$130
Transactions

Stores buy and sell records.

Field	Description
transaction_id	Transaction ID
stock_id	Stock identifier
quantity	Number of shares
action	BUY / SELL
Portfolio

Stores user stock holdings.

Field	Description
portfolio_id	Portfolio ID
user_id	User identifier
stock_id	Stock identifier
quantity	Shares owned
Application Pages

Home Page

Signup Page

Login Page

Trader Dashboard

Admin Dashboard

Portfolio Page

Buy Stock Page

Sell Stock Page

Project Folder Structure
stocker
│
├── app.py
├── db.py
├── requirements.txt
│
├── templates
│   ├── index.html
│   ├── login.html
│   ├── signup.html
│   ├── dashboard.html
│   ├── admin_dashboard.html
│
└── static
    └── style.css
