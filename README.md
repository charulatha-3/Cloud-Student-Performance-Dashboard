# ☁️ Cloud Student Performance Dashboard

A modern web-based **Student Performance Management and Analytics Dashboard** designed to monitor student academic performance, analyze subject-wise results, and manage student records.

The project uses a responsive dashboard interface with a **dark navy, cyan, and purple analytics theme**.

> **Note:** This version is an educational prototype. Student data is stored in the browser using `localStorage`. It is not connected to AWS cloud services yet.

---

## 📌 Project Overview

The **Cloud Student Performance Dashboard** helps educational institutions monitor and analyze student academic performance through a centralized dashboard.

Administrators can:

* View the total number of students
* Monitor average academic performance
* Identify excellent-performing students
* Identify students who need attention
* View subject-wise performance
* Search student records
* Filter students by performance grade
* Add new students
* Edit student information
* Delete student records
* Export student data as JSON
* Store prototype data using browser `localStorage`

---

## 🎯 Objectives

* Create a centralized student performance management system.
* Provide quick academic performance statistics.
* Analyze subject-wise performance.
* Identify high-performing and low-performing students.
* Provide an easy-to-use administrative dashboard.
* Demonstrate how the application can later be connected to cloud services.

---

## ✨ Features

### 📊 Dashboard

The dashboard displays:

* Total Students
* Average Performance
* Excellent Students
* Students Needing Attention

### 📈 Performance Analytics

Subject performance is displayed using:

* Performance bars
* Percentage indicators
* Subject-wise averages

### 👨‍🎓 Student Management

Administrators can:

* Add students
* Edit students
* Delete students
* Search students
* Filter students

### 🏆 Grade Classification

Students are automatically classified according to their percentage:

| Percentage | Grade     |
| ---------- | --------- |
| 85% – 100% | Excellent |
| 70% – 84%  | Good      |
| 50% – 69%  | Average   |
| Below 50%  | Low       |

### ☁️ Data Storage

The prototype uses browser `localStorage` to preserve student records after refreshing the page.

### 📥 Data Export

Student information can be exported as a JSON file.

---

## 🛠️ Technologies Used

### Frontend

* HTML5
* CSS3
* JavaScript

### Storage

* Browser LocalStorage

### Development Tool

* Visual Studio Code

### Future Cloud Technologies

* AWS Amplify
* Amazon Cognito
* Amazon API Gateway
* AWS Lambda
* Amazon DynamoDB
* Amazon CloudFront

---

## 🏗️ Proposed Cloud Architecture

The current project is a frontend prototype.

The planned cloud architecture is:

```text
                ┌─────────────────────┐
                │       Student       │
                │     / Admin User    │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │   AWS Amplify /     │
                │    CloudFront       │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │   Cloud Dashboard   │
                │    HTML/CSS/JS      │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │   API Gateway       │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │    AWS Lambda       │
                │ Business Logic      │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │    DynamoDB         │
                │ Student Records     │
                └─────────────────────┘

                ┌─────────────────────┐
                │   Amazon Cognito    │
                │ Authentication      │
                └─────────────────────┘
```

---

## 📂 Project Structure

```text
CloudStudentDashboard/
│
├── index.html
│
└── README.md
```

---

## 🚀 How to Run

### Step 1 — Create the Folder

Create a folder named:

```text
CloudStudentDashboard
```

### Step 2 — Open in VS Code

Open the folder using:

```text
VS Code → File → Open Folder → CloudStudentDashboard
```

### Step 3 — Create the HTML File

Create:

```text
index.html
```

Paste the complete project code into the file.

### Step 4 — Run the Project

You can open `index.html` directly in a browser.

For a better development experience, install the **Live Server** extension in VS Code and select:

```text
Right Click → Open with Live Server
```

The dashboard will open in your browser.

---

## 💾 Local Storage

The application stores student information using:

```javascript
localStorage
```

The storage key is:

```text
cloudStudentPerformance
```

This allows the student records to remain available after refreshing the browser.

---

## 👨‍🎓 Sample Student Data

The project includes sample records such as:

| Student       | Department             | Year     | Percentage |
| ------------- | ---------------------- | -------- | ---------: |
| Aarav Kumar   | Computer Science       | 3rd Year |        91% |
| Meera Sharma  | Information Technology | 3rd Year |        86% |
| Rahul Raj     | Computer Science       | 2nd Year |        78% |
| Diya Nair     | Electronics            | 4th Year |        94% |
| Vikram Das    | Mechanical             | 3rd Year |        68% |
| Ananya Rao    | Computer Science       | 2nd Year |        83% |
| Karthik Kumar | Information Technology | 4th Year |        72% |

---

## ☁️ AWS Cloud Implementation

For a real cloud-based implementation, the frontend can be deployed using **AWS Amplify** or **Amazon CloudFront**.

Student authentication can be implemented using **Amazon Cognito**.

The application can communicate with backend APIs through **Amazon API Gateway**.

Business logic can be processed using **AWS Lambda**.

Student records can be stored in **Amazon DynamoDB**.

### Proposed Flow

```text
Admin Login
     ↓
Amazon Cognito
     ↓
Cloud Dashboard
     ↓
API Gateway
     ↓
AWS Lambda
     ↓
DynamoDB
     ↓
Student Performance Data
```

---

## 🔐 Security Improvements for Cloud Version

The prototype does not implement production-level security.

For a real deployment, the following can be added:

* Amazon Cognito authentication
* Role-based access control
* HTTPS
* API authorization
* DynamoDB access policies
* AWS IAM permissions
* Data encryption
* Secure API endpoints
* Audit logs
* Backup and recovery

---

## 🔮 Future Enhancements

The project can be extended with:

* 👨‍🏫 Teacher login
* 👨‍🎓 Student login
* 🔐 Admin authentication
* ☁️ Real-time cloud synchronization
* 📧 Email notifications
* 📱 Mobile-responsive PWA
* 📊 Advanced performance charts
* 📄 PDF report generation
* 📈 Semester-wise analytics
* 🏫 Department-wise analytics
* 📝 Attendance integration
* 🎯 Academic performance prediction
* 🤖 AI-based student performance prediction
* 🔔 Low-performance alerts
* ☁️ AWS cloud database integration

---

## 🤖 Possible AI Extension

An AI/ML module can be added to predict students who may require academic support.

Possible input parameters:

```text
Attendance
Internal Marks
Assignment Scores
Previous Semester Marks
Lab Performance
Exam Scores
```

The system could generate:

```text
Performance Risk
        ↓
Low Risk
Medium Risk
High Risk
```

This could help faculty identify students who may need additional academic support.

---

## 📊 Example Dashboard

The dashboard provides:

```text
┌─────────────────────────────────────────────┐
│       CLOUD STUDENT PERFORMANCE             │
├────────────┬────────────┬───────────────────┤
│ Students   │ Average    │ Excellent         │
│    7       │   81.7%    │    4              │
├────────────┴────────────┴───────────────────┤
│                                             │
│       Subject Performance Analytics         │
│                                             │
├─────────────────────────────────────────────┤
│ Student Records                             │
│                                             │
│ Search | Filter | Add Student               │
│                                             │
└─────────────────────────────────────────────┘
```

---

## 🎓 Academic Use

This project can be used as a:

* Cloud Computing Mini Project
* Web Development Project
* Database Project Prototype
* College Mini Project
* CSE Academic Project
* AWS Cloud Project Prototype

---

## ⚠️ Disclaimer

This project is an **educational prototype**.

The current version uses browser `localStorage` and does not provide:

* Real cloud synchronization
* Production authentication
* Secure medical/academic data storage
* Multi-user access control
* Server-side database storage

For production deployment, the application should be connected to appropriate AWS services with proper authentication, authorization, encryption, and security policies.

---

## 👩‍💻 Author

**Charulatha S**

B.E. Computer Science Engineering
Prathyusha Engineering College

---

## ⭐ Project Highlights

```text
Modern Dashboard
      +
Student Management
      +
Performance Analytics
      +
Local Data Storage
      +
Cloud Architecture
      +
AWS Deployment Plan
```

**Cloud Student Performance Dashboard — Turning student data into meaningful academic insights.**
