# BusPassSystem
#  Cloud-Based Bus Pass System

This project is a simple, serverless **Bus Ticket Booking System** built using **AWS services** for frontend hosting, backend processing, and data storage. Developed as part of the **CodeAlpha Internship**, this project demonstrates full-stack deployment on the cloud using minimal infrastructure.

---

##  Technologies Used

| Layer       | Tool/Service        |
|-------------|---------------------|
| Frontend    | HTML, CSS, JavaScript (hosted on **AWS S3**) |
| Backend     | **AWS Lambda** (Python) via **API Gateway** |
| Database    | **Amazon DynamoDB** |
| Deployment  | Git, GitHub, Git Bash, AWS CLI |



>  [Click here to view the hosted site](http://bus-pass-system-site.s3-website-us-east-1.amazonaws.com)


## 📸 Screenshot:<img width="844" height="482" alt="image" src="https://github.com/user-attachments/assets/349145ad-47bc-4ded-80f8-bd8da3311ed8" />:<img width="1004" height="348" alt="image" src="https://github.com/user-attachments/assets/cc94ffff-167c-49b5-8f73-912e6569c1ed" />:<img width="1013" height="419" alt="image" src="https://github.com/user-attachments/assets/2d663ece-7450-4eb7-8f76-d62477137b12" />:<img width="999" height="429" alt="image" src="https://github.com/user-attachments/assets/c7f5cd00-64c5-4302-9d8a-35c692cf145e" />:<img width="896" height="469" alt="image" src="https://github.com/user-attachments/assets/3989a542-9300-4a08-ac6f-01c85f931fd5" />:<img width="997" height="472" alt="image" src="https://github.com/user-attachments/assets/631a88eb-3fb6-4c9f-9b15-d83dbc44d44b" />:<img width="1362" height="539" alt="image" src="https://github.com/user-attachments/assets/8bd45d1a-90aa-44e4-8397-e3da1fa5c75d" />:<img width="947" height="246" alt="image" src="https://github.com/user-attachments/assets/f33fdb0c-3bb7-4aa9-a4e0-b0582c5d50c1" />






##  How It Works

1. User fills in name, destination, and number of tickets
2. On form submission, data is sent to AWS Lambda via API Gateway
3. Lambda function writes booking details to DynamoDB
4. User receives a success message with a booking ID

---

##  Folder Structure

```

BusPassSystem/
├── index.html
├── style.css
├── script.js
└── README.md

````

---

##  Setup Instructions

### 1. AWS Setup

- Create a DynamoDB Table: `BusBookings` with partition key `bookingId` (String)
- Deploy a Lambda Function using Python (see full guide in repo)
- Create an API Gateway to expose your Lambda via HTTP

### 2. Upload Frontend to S3

```bash
aws s3 cp index.html s3://bus-pass-website --acl public-read
aws s3 cp style.css s3://bus-pass-website --acl public-read
aws s3 cp script.js s3://bus-pass-website --acl public-read
````

---

##  Deployment via Git Bash

```bash
git init
git add .
git commit -m "Bus Pass System for CodeAlpha"
git branch -M main
git remote add origin https://github.com/annameggison/BusPassSystem.git
git push -u origin main
```

---

##  Credits

* Project by: \Anna Meggison
* Internship: [CodeAlpha Internship](https://codealpha.tech/)
* Tools: AWS, GitHub, Git Bash

---

##  Contact:talktofaasema@gmail.com






