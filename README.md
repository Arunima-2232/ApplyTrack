# ApplyTrack
Internship &amp; Job Application Tracking System

## Vision Document

### Project Name:
ApplyTrack - Internship and Job Application Tracking System

### Overview:
A web-based application tracking system that provides to students and job seekers a unified platform to monitor application status, review past applications, identify suitable opportunities and respond to updates in a timely manner. It also allows recruiters to manage large volumes of applications efficiently, enforce deadlines and communicate updates to applicants.

### Problem It Solves:
There is no unified, user-centric system that enables applicants to track applications, monitor application status and receive timely notifications, while also allowing recruiters to post opportunities, review applications, and manage application lifecycles efficiently. The absence of such a centralized platform leads to missed deadlines, poor visibility of application outcomes and inefficient communication between applicants and recruiters.

### Target Users:
1. Primary Users: Students and Job Applicants
2. Secondary Users: Recruiters, Administrator
3. System Users: Notification System

### Vision Statement:
ApplyTrack aims to become a user-friendly and trustworthy platform that helps applicants manage their job and internship applications in one place. It focuses on improving transparency and organization through real-time tracking and personalized recommendations.

### Key Features/Goals:
Develop a lightweight, web-based Application Tracking System (ATS) that provides a centralized platform for managing internship and job applications by supporting the following:

1. Allow applicants to create and manage user accounts containing personal details and application history
2. Enable applicants to view applicable opportunities and receive recommended opportunities based on profile details
3. Allow applicants to apply for opportunities, track application status, and view results when published
4. Provide recruiters with functionality to post opportunities, view submitted applications, and manage application status
5. Enable administrators to manage user accounts, opportunities, and overall system activity
6. Integrate a notification mechanism to inform users about application updates, deadlines, and system events

### Success Metrics:

1. Applicants can successfully manage and track applications
2. Recruiters can post and manage opportunities efficiently
3. Notifications are delivered accurately and on time
4. The system reflects correct application statuses and results
5. At least 80% of test users can use the system without assistance
6. The project is completed within the defined timeline

### Assumptions:

1. Users have access to a web browser and internet connectivity
2. Applicants are willing to maintain their application records
3. Recruiters will update application statuses when required
4. The notification system is available and operational

### Constraints:

1. Only open-source tools and technologies will be used
2. The system must be scalable enough to support multiple users
3. User data must be handled securely and confidentially
4. The system must be developed within the given timeframe

### MoSCoW Prioritization

Must Have: Core authentication, application tracking, job posting  
Should Have: Notifications, recommendations, profile management  
Could Have: Analytics, filters, UI customization  
Won’t Have: AI analysis, video interviews, mobile app

### Technology Stack

1. Frontend - Streamlit is used to develop the web-based user interface for ApplyTrack. It is responsible for displaying login pages, dashboards, job listings, and application status.
2. Backend - Flask is used as the backend framework to handle API requests, authentication, and business logic. Python is used as the primary programming language.
3. Database - Supabase is used as the cloud-based PostgreSQL database for storing user data, job details, applications, and system records.
4. Development and Deployment Tools - Docker is used for containerization. GitHub is used for version control and project management. Figma is used for wireframe design. Draw.io is used for architecture diagrams.
5. Development Environment - VS Code is used as the code editor. Command Prompt or PowerShell is used for executing development commands. Docker Desktop is used for managing containers.

### System Workflow

1. Users such as applicants, recruiters, and administrators access the system through a web browser.
2. The frontend interface is loaded using the Streamlit framework.
3. User requests such as login, registration, job application, and status tracking are sent to the Flask backend using HTTP APIs.
4. The backend server validates the requests and executes business logic.
5. The backend communicates with the Supabase database to store and retrieve information.
6. Processed data is sent back from the backend to the frontend.
7. Notifications are generated for important updates such as application status changes.
8. The final output is displayed to the user in real time.

### Branching Strategy

1. The project follows the GitHub Flow branching strategy.
2. The main branch contains stable and production-ready code.
3. New features are developed in separate feature branches created from the main branch.
4. Feature branches follow the naming format:
    feature-featureName
5. Developers create a feature branch, implement changes, test the feature, and then merge it into the main branch.
6. This strategy helps maintain code stability and organized development.

### Docker Setup for Local Development

1. Docker Desktop must be installed on the system before starting.
2. The project contains the following required files: Dockerfile, requirements.txt, and app.py.
3. To build the Docker image, open Command Prompt or PowerShell in the project directory and run: docker build -t applytrack .
4. To run the Docker container, execute: docker run -p 8501:8501 applytrack
5. After running the container, open a web browser and visit: http://localhost:8501
6. Docker ensures a consistent development environment and reduces dependency conflicts.
