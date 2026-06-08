# ACADEMIC PROJECT TRACKING AND MANAGEMENT PORTAL

## 1. Project Title Finalization

**Project Title:** Academic Project Tracking and Management Portal

The title was selected to clearly represent the primary purpose of the application — managing, monitoring, and tracking academic projects throughout their lifecycle. The system provides a centralized platform for students, faculty guides, and administrators to handle project submissions, progress tracking, reviews, evaluations, and documentation efficiently.

---

## 2. Requirement Gathering

Requirement gathering involves identifying the needs of users and understanding the challenges faced in managing academic projects manually. Many educational institutions rely on spreadsheets, emails, and paper-based records, which can lead to inefficiencies and difficulties in monitoring project activities.

### Functional Requirements

* Student Registration and Login
* Faculty and Admin Login
* Project Proposal Submission
* Guide Assignment
* Progress Tracking
* Project Document Upload
* Review and Feedback Management
* Project Evaluation
* Report Generation
* Dashboard Monitoring

### Non-Functional Requirements

* User-Friendly Interface
* Secure Data Storage
* Fast System Performance
* Data Accuracy and Reliability
* Scalability for Future Enhancements
* Role-Based Access Control

---

## 3. Objective Definition

The main objectives of the Academic Project Tracking and Management Portal are:

* To digitize academic project management activities.
* To reduce manual paperwork and administrative effort.
* To provide real-time project monitoring and status tracking.
* To improve communication between students and faculty guides.
* To maintain project records securely.
* To generate project reports and evaluation summaries efficiently.
* To enhance transparency in project review and assessment processes.

---

## 4. User Identification

The system is designed for the following users:

### Student

* Submit project proposals
* Upload project reports and documents
* View project status
* Track progress updates
* View guide feedback

### Faculty Guide

* Review project proposals
* Monitor assigned projects
* Provide comments and feedback
* Evaluate project progress
* Approve submissions

### Administrator

* Manage students and faculty accounts
* Assign guides to projects
* Monitor overall project activities
* Generate project reports
* Manage system operations

---

## 5. Module Identification

### User Management Module

Handles user registration, authentication, and role-based access control.

### Project Proposal Module

Allows students to submit project proposals and project information.

### Guide Assignment Module

Facilitates allocation of faculty guides to projects.

### Progress Tracking Module

Monitors project milestones, updates, and completion status.

### Document Management Module

Handles uploading, storing, and accessing project documents and reports.

### Review & Feedback Module

Enables faculty guides to review projects and provide recommendations.

### Project Evaluation Module

Maintains project assessment records and evaluation details.

### Dashboard Module

Provides a summarized view of project activities, status, and statistics.

### Reporting Module

Generates project progress reports, evaluation reports, and completion summaries.

---

## 6. UML Diagram Description

### 6.1 Use Case Diagram

The Use Case Diagram illustrates how different users interact with the system.

#### Actors

* Student
* Faculty Guide
* Administrator

#### Use Cases

* Login
* Submit Project Proposal
* Upload Documents
* Track Progress
* Assign Guide
* Review Project
* Provide Feedback
* Evaluate Project
* Generate Reports

#### Explanation

* Students can submit and monitor projects.
* Faculty guides can review and evaluate assigned projects.
* Administrators manage users, guides, and project activities.
* The diagram represents the interaction between users and the system functionalities.

---

### 6.2 Class Diagram

#### Classes

### Student

* studentId
* studentName
* email
* department

Functions:

* login()
* submitProject()
* uploadDocument()

### Project

* projectId
* projectTitle
* domain
* status

Functions:

* createProject()
* updateStatus()

### Guide

* guideId
* guideName
* department

Functions:

* reviewProject()
* provideFeedback()

### Progress

* progressId
* milestone
* remarks

Functions:

* addProgress()
* updateProgress()

### Report

* reportId
* reportType

Functions:

* generateReport()

#### Relationships

* One Student can have multiple Projects.
* One Guide can supervise multiple Projects.
* One Project can have multiple Progress Updates.
* Reports are generated from Project and Progress data.

---

### 6.3 UML Design Considerations

* Modular system architecture
* Easy maintenance and scalability
* Clear separation of functionalities
* Proper relationship management
* Standard UML design principles

---

# Data Requirement Analysis

## 1. Overview

Data Requirement Analysis identifies the data required to manage academic projects effectively. The system stores project information, user details, progress updates, reviews, and evaluation records.

---

## 2. Types of Data Required

### a) Student Data

* Student ID
* Student Name
* Department
* Email
* Password

### b) Faculty Guide Data

* Guide ID
* Guide Name
* Department
* Email

### c) Project Data

* Project ID
* Project Title
* Domain
* Description
* Status
* Submission Date

### d) Progress Data

* Progress ID
* Project ID
* Milestone
* Remarks
* Update Date

### e) Evaluation Data

* Evaluation ID
* Project ID
* Marks
* Feedback
* Review Date

---

## 3. Data Sources

The system collects data from:

* Student project submissions
* Faculty reviews and evaluations
* Administrator management activities
* Project progress updates

---

## 4. Data Storage Requirements

* Store data in a MySQL database
* Maintain unique IDs for all entities
* Support fast retrieval and updates
* Maintain relationships between users, projects, and evaluations

---

## 5. Data Processing Requirements

The system should support:

* Project creation and updates
* Guide assignment
* Progress tracking
* Document management
* Evaluation management
* Report generation

---

## 6. Data Integrity & Validation

* Unique IDs for all records
* Mandatory fields validation
* Secure authentication
* Data consistency checks
* Prevention of duplicate records

---

## 7. Data Security Requirements

* Role-based access control
* Secure password storage
* Controlled access to project records
* Backup and recovery support

---

## 8. Data Relationships

* One Student → Multiple Projects
* One Guide → Multiple Projects
* One Project → Multiple Progress Records
* One Project → Multiple Evaluation Records
* Administrators manage all project-related information
