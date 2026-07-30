# Enterprise Healthcare Campaign Platform
### Technical Case Study

> **Confidential Client Project**

This repository showcases the technical architecture, engineering approach, and production experience behind an enterprise healthcare campaign platform that I developed for a client.

The original production application and its source code are **not included** in this repository due to client confidentiality and intellectual property restrictions.

Instead, this repository demonstrates:

- Enterprise application architecture
- Video processing workflow
- Dashboard design and system workflow
- Production support experience
- Technical documentation
- Public campaign highlights
- Related open-source implementations

## 📖 Project Overview

This repository presents a technical case study of an enterprise healthcare campaign platform developed for a client as part of a nationwide healthcare awareness initiative.

The platform was designed to streamline campaign execution by enabling large-scale doctor onboarding, centralized management, automated branded video generation, reporting, and day-to-day operational support through a secure web application.

To respect client confidentiality and intellectual property, the production source code is not included in this repository. Instead, this repository focuses on the overall system architecture, development approach, workflows, technical challenges, and engineering experience gained while delivering the solution.

---

## 👨‍💻 My Role

I worked as the software developer responsible for designing, developing, deploying, and supporting the application throughout the campaign lifecycle.

My primary responsibilities included:

- Designing and developing the web application
- Building frontend and backend modules
- Implementing secure authentication and user management
- Developing the video processing workflow
- Integrating background job processing
- Managing production deployment and server configuration
- Providing production support during the live campaign
- Troubleshooting issues reported by managers and campaign teams
- Preparing technical documentation and user guidance
- Coordinating with the client to deliver feature enhancements and issue resolutions

Throughout the project, the focus was on delivering a stable, scalable, and reliable platform for day-to-day campaign operations.

> **Note:** This repository showcases my technical contribution to the project. The campaign, application, and associated recognitions belong to the client. No confidential source code, business data, or proprietary implementation details are included.

---

# 🛠️ Technology Stack

The platform was developed using a modern full-stack architecture designed to support secure, scalable, and high-performance enterprise operations.

## Frontend

The user interface was developed using **Next.js**, providing a responsive, server-rendered, and performance-optimized web experience. The frontend was designed to support multiple user roles while ensuring smooth navigation and efficient application performance.

**Technology Used**
- Next.js

---

## Backend

The backend is built with **Next.js**, responsible for handling business logic, REST APIs, authentication, data processing, and server-side operations. It serves as the core application layer connecting users, services, and the database.

**Technology Used**
- Next.js

---

## Database

The application uses **MongoDB** as its primary database for storing and managing operational data.

The database is responsible for:

- User information
- Doctor records
- Campaign-related data
- Application metadata
- System-generated information

**Technology Used**
- MongoDB

---

## Authentication & Security

Authentication is implemented using **JWT (JSON Web Token)** to ensure secure access to protected resources.

Security features include:

- Secure user authentication
- Token-based authorization
- Protected API access
- Session validation

**Technology Used**
- JWT (JSON Web Token)

---

## Hosting Infrastructure

The production application is hosted on a **Hostinger VPS**, providing a dedicated server environment with greater control over deployment, scalability, and server management.

### Approximate Server Configuration

| Component | Specification |
|-----------|---------------|
| CPU | 2 vCPU Cores |
| RAM | 8 GB |
| Storage | 100 GB NVMe SSD |
| Bandwidth | 8 TB |

---

## Deployment & Server Management

The production environment uses multiple technologies to ensure application stability, process management, and efficient request routing.

### PM2

Used for:

- Application process management
- Automatic restart on failure
- Performance monitoring
- High application availability

### Nginx

Used for:

- Reverse proxy configuration
- Request routing
- Static file serving
- Load handling

### Docker

Used for:

- Application containerization
- Environment consistency
- Simplified deployment
- Dependency isolation

---

# ⚙️ Major Integrations

The application integrates multiple technologies to support campaign operations.

## FFmpeg

FFmpeg is used for automated video processing and generation, enabling branded campaign videos to be created programmatically.

---

## Email Integration

Email services are integrated to support automated communication and notification workflows within the application.

---

## Excel Integration

Excel functionality is used for:

- Data import
- Data export
- Bulk record management
- Reporting

---

# 🚀 Background Processing

The application uses **BullMQ** for background job processing and queue management.

Resource-intensive operations such as video generation are executed asynchronously instead of during user requests.

This architecture provides several advantages:

- Efficient queue management
- Controlled concurrency
- Better resource utilization
- Improved application responsiveness
- Reduced server load during heavy processing

By processing video-generation jobs in the background, the platform ensures that long-running tasks do not block normal user interactions, resulting in a more stable and scalable application.

---

# 🏗️ Technical Architecture Highlights

The platform combines modern web technologies to support both standard web operations and computationally intensive media-processing workflows.

Key architectural capabilities include:

- Enterprise web application architecture
- Secure authentication using JWT
- MongoDB-based data management
- Containerized deployment using Docker
- Reverse proxy configuration with Nginx
- Process management through PM2
- Automated video generation with FFmpeg
- Background task execution using BullMQ
- Queue-based concurrency management
- Scalable VPS hosting environment

Together, these technologies provide a structured and reliable foundation for secure application management, automated media processing, efficient background task execution, and smooth day-to-day campaign operations.

# ✨ Key Features

The platform was developed to support the complete lifecycle of a large-scale healthcare awareness campaign by providing secure, efficient, and automated digital operations.

## 🔐 Secure User Authentication

- JWT-based authentication
- Role-based user access
- Protected application routes
- Secure session management

---

## 👥 User & Manager Management

The platform supports multiple user roles with controlled access to different modules.

Key capabilities include:

- User registration and management
- Role-based permissions
- Manager-wise data access
- Secure account management

---

## 🩺 Doctor Management

A centralized module was developed to manage doctor-related campaign activities.

Features include:

- Doctor registration
- Profile management
- Data verification
- Record updates
- Search and filtering
- Bulk data handling

---

## 🎥 Automated Video Generation

One of the primary capabilities of the platform is automated branded video generation.

The system processes campaign assets and generates personalized videos using background processing techniques.

Core technologies include:

- FFmpeg
- BullMQ
- Background Job Queue
- Queue Management
- Concurrent Processing

---

## 📊 Dashboard & Reporting

The application provides dashboards to monitor campaign progress and operational activities.

Key capabilities:

- Campaign monitoring
- Operational reporting
- Data summaries
- Progress tracking
- Administrative insights

---

## 📁 Excel Import & Export

The application supports Excel-based workflows for large-scale data management.

Features include:

- Bulk data import
- Bulk data export
- Report generation
- Data validation

---

## 📧 Email Notifications

Integrated email services support automated communication within the platform.

Examples include:

- System notifications
- User communication
- Operational updates

---

## ⚡ Background Job Processing

Long-running operations are processed asynchronously to maintain application performance.

This includes:

- Video generation
- Queue management
- Background task execution
- Resource optimization
- Concurrent processing

---

## 🚀 Production Deployment

The application was deployed in a production VPS environment using modern deployment practices.

Deployment stack:

- Docker
- PM2
- Nginx
- Hostinger VPS

---

## 🛡️ Reliability & Performance

The platform was designed to support continuous campaign operations with emphasis on:

- Secure authentication
- Stable application performance
- Efficient background processing
- Scalable deployment architecture
- Reliable operational workflow

---
# 🏗️ System Architecture

## Overview

The application follows a modern full-stack architecture designed to support secure user management, high-volume campaign operations, automated media processing, and production-grade deployment.

The architecture separates user interaction, business logic, data storage, and background processing into dedicated layers to improve maintainability, scalability, and overall system performance.

---

## High-Level Architecture

```text
                    Users
                       │
                       ▼
               Next.js Frontend
                       │
                       ▼
          Next.js Backend (APIs)
                       │
      ┌────────────────┼────────────────┐
      ▼                ▼                ▼
 MongoDB          JWT Authentication   BullMQ
      │                                 │
      │                                 ▼
      │                         Background Jobs
      │                                 │
      │                                 ▼
      │                             FFmpeg
      │                                 │
      └──────────────────────┬──────────┘
                             ▼
                     Generated Videos

Deployment Layer
Docker → PM2 → Nginx → Hostinger VPS
```

---

## Architecture Components

### 🖥️ Frontend Layer

The frontend is built using **Next.js**, providing a fast, responsive, and user-friendly interface for campaign users.

Its responsibilities include:

- User interaction
- Form handling
- Dashboard rendering
- Report visualization
- Secure communication with backend APIs

---

### ⚙️ Backend Layer

The backend is responsible for all server-side operations.

Responsibilities include:

- Business logic
- REST APIs
- Authentication
- Authorization
- Database communication
- Queue management
- Video generation requests

---

### 🗄️ Database Layer

MongoDB stores the operational data required by the application.

Examples include:

- User records
- Doctor information
- Campaign data
- Generated video metadata
- Operational information

---

### 🔐 Authentication Layer

JWT authentication protects application resources by validating user identity before allowing access to protected APIs and modules.

---

### 🎥 Media Processing Layer

Video processing is handled using FFmpeg.

Instead of generating videos during live user requests, tasks are processed asynchronously using BullMQ.

This approach:

- Improves performance
- Reduces request waiting time
- Prevents server blocking
- Supports multiple simultaneous processing requests

---

### 🚀 Deployment Layer

The production environment uses multiple infrastructure components.

| Technology | Purpose |
|------------|---------|
| Docker | Containerized deployment |
| PM2 | Process management |
| Nginx | Reverse proxy & request routing |
| Hostinger VPS | Production hosting |

---

## Design Principles

The architecture was designed with the following objectives:

- Scalability
- Reliability
- Security
- Maintainability
- Efficient background processing
- High availability
- Separation of responsibilities
- Performance optimization

---

## Confidentiality Notice

This diagram represents a **high-level conceptual architecture** intended for technical documentation and portfolio purposes.

Specific implementation details, proprietary business logic, internal APIs, database schemas, and production configurations have been intentionally omitted to respect client confidentiality and intellectual property.

# 🔄 Project Workflow

## Overview

The platform follows a structured workflow that guides campaign operations from user authentication to automated video generation and reporting. Each stage is designed to ensure secure access, efficient data management, and reliable execution of resource-intensive tasks.

---

## Workflow Diagram

```text
User Login
     │
     ▼
JWT Authentication
     │
     ▼
Dashboard Access
     │
     ▼
Doctor Data Management
     │
     ▼
Data Validation
     │
     ▼
Video Generation Request
     │
     ▼
BullMQ Queue
     │
     ▼
FFmpeg Video Processing
     │
     ▼
Generated Video
     │
     ▼
Reports & Campaign Tracking
```

---

## Step 1 – User Authentication

Users securely log in to the platform using JWT-based authentication. After successful verification, they are granted access according to their assigned role and permissions.

---

## Step 2 – Dashboard Access

Authenticated users access their dashboard, where they can perform campaign-related operations based on their role.

Examples include:

- Managing doctor records
- Monitoring campaign progress
- Accessing reports
- Performing operational tasks

---

## Step 3 – Doctor Data Management

The platform provides centralized management of doctor information.

Typical operations include:

- Adding new records
- Updating existing records
- Searching and filtering data
- Managing campaign-related information

---

## Step 4 – Data Validation

Before initiating automated processing, the application validates the submitted data to ensure completeness and consistency.

This helps reduce processing errors and maintain data quality.

---

## Step 5 – Video Generation Request

When a video generation request is submitted, the application prepares the required information and sends the task to the background processing queue instead of processing it immediately.

This approach prevents long-running tasks from blocking user interactions.

---

## Step 6 – Background Queue Processing

BullMQ manages incoming video generation requests by placing them into a processing queue.

This enables:

- Controlled concurrency
- Reliable task execution
- Efficient workload distribution
- Better server performance

---

## Step 7 – Video Processing

Queued jobs are processed using FFmpeg to generate campaign-branded videos.

The generated output is stored and made available for campaign use.

---

## Step 8 – Campaign Monitoring & Reporting

Throughout the campaign, the platform provides dashboards and reporting capabilities to help monitor operational activities and campaign progress.

Reports support data analysis, operational tracking, and day-to-day management.

---

## Workflow Objectives

The workflow was designed to achieve the following goals:

- Secure access control
- Centralized campaign management
- Efficient doctor data handling
- Automated media generation
- Reliable background processing
- Scalable system performance
- Smooth production operations

---

## Engineering Considerations

The workflow emphasizes scalability and operational stability by separating user-facing activities from resource-intensive background processing. This design helps maintain a responsive application while supporting large-scale campaign operations.

# 🚀 Production Support

## Overview

Beyond application development, I was actively involved in supporting the platform during the live campaign. This included monitoring production operations, resolving technical issues, coordinating with stakeholders, and ensuring the platform remained available for day-to-day campaign activities.

The objective was to deliver a stable and reliable experience while minimizing operational disruptions.

---

## My Responsibilities

During production, I was responsible for:

- Monitoring application health and availability
- Troubleshooting reported technical issues
- Investigating user-reported problems
- Supporting managers during campaign operations
- Coordinating issue resolution with the technical team
- Assisting with production deployments
- Preparing user guidance and documentation
- Creating tutorial videos for platform users
- Providing technical support throughout the campaign

---

## Production Issue Resolution

During the live campaign, several operational issues required investigation and resolution.

Examples of the types of issues handled include:

- User access issues
- Login-related troubleshooting
- Network and connectivity problems
- Browser compatibility issues
- Data validation support
- Video processing requests
- Deployment-related verification
- General production support

Each issue was analyzed, diagnosed, and resolved while minimizing the impact on campaign operations.

---

## User Support

The platform supported a large number of operational users.

Support activities included:

- Assisting campaign managers
- Explaining platform workflows
- Resolving operational queries
- Guiding users through application features
- Helping users complete campaign activities successfully

To improve user adoption, technical guidance and tutorial resources were also prepared for end users.

---

## Operational Focus

The production support process emphasized:

- Reliability
- Stability
- Fast issue resolution
- Clear communication
- Continuous monitoring
- User assistance
- Operational continuity

---

## Key Learnings

Working on a live production campaign provided valuable experience in:

- Enterprise application support
- Production troubleshooting
- Incident analysis
- Technical communication
- Cross-functional collaboration
- Live deployment management
- User-centric problem solving

The experience reinforced the importance of building software that is not only functional but also maintainable, reliable, and well-supported throughout its operational lifecycle.

# 📊 Project Impact

## Project Scope

This platform was developed to support a large-scale healthcare awareness campaign by providing a centralized web application for campaign management, operational coordination, automated media generation, and reporting.

The application was designed to streamline day-to-day campaign activities while maintaining security, reliability, and operational efficiency.

---

## Engineering Highlights

During the project, the platform included capabilities such as:

- Secure role-based authentication
- Centralized doctor data management
- Automated branded video generation
- Background job processing using BullMQ
- Queue-based media processing with FFmpeg
- Production deployment on a VPS environment
- Dashboard-based monitoring and reporting
- Excel import and export workflows
- Email notification integration
- Production support throughout the campaign

---

## Technical Objectives

The engineering goals of the platform included:

- Building a scalable web application
- Automating repetitive operational tasks
- Improving campaign execution efficiency
- Maintaining application responsiveness during media processing
- Supporting secure multi-user access
- Providing a stable production environment
- Simplifying campaign management workflows

---

## Professional Experience Gained

Working on this project provided hands-on experience in:

- Enterprise application development
- Full-stack web engineering
- Production deployments
- Background job processing
- Media processing automation
- Technical troubleshooting
- Production support
- Cross-functional collaboration
- Technical documentation
- Client communication

---

## Repository Purpose

This repository has been created as a technical case study to showcase the engineering approach, architecture, workflows, and lessons learned while developing and supporting an enterprise healthcare campaign platform.

To respect client confidentiality, proprietary source code, production data, internal documentation, and business-specific implementation details have been intentionally excluded.

