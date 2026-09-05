# Jisr Platform

**Jisr Platform** is an AI-powered career development and talent-matching ecosystem designed to bridge the gap between university students and the job market.

The platform connects **students, companies, supervisors, and mentors** through practical projects, job and internship opportunities, skill assessment, CV analysis, market insights, smart candidate ranking, mentoring, communication, and progress-tracking workflows.

> This repository contains the **Flutter mobile application** for Jisr Platform, including the Student and Company experiences.

---

## Overview

Jisr was built as a graduation project to provide a practical environment where students can develop verified skills, build a professional profile, work on real opportunities, and connect with companies.

Companies can publish opportunities, review candidates, use smart ranking, communicate with students, follow task progress, and evaluate completed work.

The broader Jisr ecosystem also includes supervisor, mentor, and administrative workflows.

---

## Main Platform Modules

### Student Experience
- Account registration, login, OTP verification, and password recovery
- CV upload and analysis
- Skill extraction and assessment
- Student profile and portfolio
- Opportunities discovery and applications
- Tasks, internships, and jobs
- Market analysis and in-demand skills
- AI-powered chatbot support
- Mentor recommendations and mentor details
- Notifications and Firebase Cloud Messaging
- Contextual chat and communication
- Progress and submission workflows

### Company Experience
- Company registration and profile management
- Company dashboard
- Create and manage Tasks, Internships, and Jobs
- Review opportunity applicants
- Smart candidate ranking
- Candidate profile inspection
- Search students by name or skill
- Task assignment workspace
- Progress tracking
- Submission review
- Student evaluation
- Mentor nomination workflows
- Notifications
- Contextual chat

### Supervisor & Mentor Ecosystem
- Project and task supervision
- Student progress follow-up
- Student evaluation
- Professional mentoring
- Career guidance
- Project and CV review

---

## AI & Intelligent Features

Jisr integrates intelligent features to improve student development and candidate discovery, including:

- CV analysis
- Skill extraction
- Skill assessment
- Job-market analysis
- Opportunity matching
- Smart candidate ranking
- AI chatbot assistance
- Career guidance support

The platform uses AI as an **assistive layer** for analysis and recommendation while keeping important decisions under the control of students, companies, supervisors, and mentors.

---

## Key Workflows

### Student Workflow

```text
Register / Login
      ↓
Upload CV
      ↓
Analyze Skills
      ↓
Complete Assessments
      ↓
Build Professional Profile
      ↓
Explore Opportunities
      ↓
Apply
      ↓
Work / Communicate
      ↓
Submit
      ↓
Receive Evaluation
```

### Company Workflow

```text
Register Company
      ↓
Create Opportunity
      ↓
Publish
      ↓
Receive Applications
      ↓
Review / Rank Candidates
      ↓
Select Candidate
      ↓
Track Work Progress
      ↓
Review Submission
      ↓
Evaluate Student
```

---

## Mobile Architecture

The Flutter application follows the **MVC (Model–View–Controller)** pattern and uses **GetX** for state management, dependency injection, and routing.

```text
lib/
├── bindings/
├── controllers/
├── core/
├── models/
├── routes/
├── services/
├── views/
└── widgets/
```

### Architectural Principles
- Views are responsible for UI rendering
- Controllers manage state and interaction flow
- Services handle API communication and external integrations
- Models represent application data
- Bindings manage dependency injection
- Reusable components reduce duplication
- Role-based flows separate Student and Company experiences

---

## Tech Stack

### Mobile
- Flutter
- Dart
- GetX
- REST APIs
- HTTP
- Firebase Core
- Firebase Cloud Messaging
- Shared Preferences
- File Picker
- Image Picker
- Flutter Animate
- Pinput
- URL Launcher

### Platform Backend / Ecosystem
- Laravel REST API
- MySQL
- Firebase Cloud Messaging
- AI-assisted analysis and recommendation services

---

## Features

- Role-based authentication
- Student and Company mobile experiences
- CV analysis
- Skill assessment
- Student professional portfolio
- Job, Internship, and Task opportunities
- Smart candidate ranking
- Candidate search
- Market analysis
- AI chatbot
- Mentor workflows
- Task assignment workspace
- Progress tracking
- Submission review
- Evaluation workflow
- In-app notifications
- Push notifications with FCM
- Light and dark themes
- Arabic-first experience with localization support
- Reusable UI components
- Loading, empty, and error states

---

## Screenshots

Screenshots will be added later under:

```text
docs/screenshots/
```

Recommended filenames:

```text
docs/screenshots/
├── student-home.png
├── cv-analysis.png
├── student-profile.png
├── market-analysis.png
├── chatbot.png
├── company-home.png
├── opportunities.png
├── smart-ranking.png
├── candidate-profile.png
├── task-workspace.png
├── notifications.png
└── dark-mode.png
```

### Student Experience

<!--
<table>
  <tr>
    <td align="center"><strong>Student Home</strong></td>
    <td align="center"><strong>CV Analysis</strong></td>
    <td align="center"><strong>Market Analysis</strong></td>
  </tr>
  <tr>
    <td><img src="docs/screenshots/student-home.png" width="240"></td>
    <td><img src="docs/screenshots/cv-analysis.png" width="240"></td>
    <td><img src="docs/screenshots/market-analysis.png" width="240"></td>
  </tr>
</table>
-->

_Screenshots coming soon._

### Company Experience

<!--
<table>
  <tr>
    <td align="center"><strong>Company Home</strong></td>
    <td align="center"><strong>Opportunities</strong></td>
    <td align="center"><strong>Smart Ranking</strong></td>
  </tr>
  <tr>
    <td><img src="docs/screenshots/company-home.png" width="240"></td>
    <td><img src="docs/screenshots/opportunities.png" width="240"></td>
    <td><img src="docs/screenshots/smart-ranking.png" width="240"></td>
  </tr>
</table>
-->

_Screenshots coming soon._

### Workflow & Communication

<!--
<table>
  <tr>
    <td align="center"><strong>Task Workspace</strong></td>
    <td align="center"><strong>Notifications</strong></td>
    <td align="center"><strong>Chatbot</strong></td>
  </tr>
  <tr>
    <td><img src="docs/screenshots/task-workspace.png" width="240"></td>
    <td><img src="docs/screenshots/notifications.png" width="240"></td>
    <td><img src="docs/screenshots/chatbot.png" width="240"></td>
  </tr>
</table>
-->

_Screenshots coming soon._

---

## Getting Started

### Prerequisites
- Flutter SDK installed
- Compatible Dart SDK
- Android Studio or VS Code
- Android emulator or physical device
- Access to the Jisr backend API
- Firebase configuration for push notifications

### Installation

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
cd YOUR_REPOSITORY
flutter pub get
flutter run
```

---

## API Configuration

The mobile application communicates with the Jisr backend through REST APIs.

API configuration is located under:

```text
lib/core/api/
```

Before running the project, configure the API base URL according to your environment.

> Do not commit private API keys, access tokens, passwords, service-account credentials, or other secrets.

---

## Firebase Configuration

Firebase is used for push-notification functionality.

To run notifications in your own environment:

1. Create or configure a Firebase project
2. Add the Android application
3. Add the required Firebase configuration files
4. Enable Firebase Cloud Messaging
5. Run the application on a supported device

---

## Authentication Flow

```text
Role Selection
      ↓
Student / Company Registration
      ↓
Login
      ↓
OTP Verification
      ↓
Role-Based Home
```

The application also supports stored authentication state and role-aware initial navigation.

---

## Localization & Theme

Jisr was designed with an **Arabic-first** mobile experience.

The application also includes:
- RTL support
- Localization-ready structure
- Light theme
- Dark theme
- Shared theme configuration

---

## Project Scope

Jisr Platform is more than a job-listing application. It is designed as a full career-development workflow that connects students, companies, supervisors, and mentors.

The system combines professional-profile development, practical experience, assessment, recruitment, mentoring, communication, and market analysis in one ecosystem.

---

## Graduation Project

Jisr Platform was developed as a graduation project in Informatics Engineering.

The complete system consists of multiple components, including:
- Flutter mobile application
- Backend REST API
- Web-based supervisor/admin experiences
- AI-assisted analysis and recommendation modules

---

## Team Contribution

Jisr Platform was developed collaboratively as a graduation project.

- **Mobile Application:** Karam & Baraa
- **Backend:** Bashar & Batoul
- **Web Application:** Ihsan

---

## Repository Scope

This repository focuses on the **Flutter mobile application**.

Some backend, web, supervisor, admin, and AI services belong to other parts of the complete Jisr Platform ecosystem.

---

## Security Notes

Before publishing or deploying the project:
- Do not commit `.env` files
- Do not commit private API keys
- Do not commit access tokens
- Do not commit passwords
- Do not commit private Firebase service-account files
- Keep sensitive configuration outside source control

---

## Future Improvements

Potential future extensions include:
- Expanded analytics dashboards
- More advanced recommendation models
- Additional assessment types
- Enhanced mentor scheduling
- More granular notification routing
- Extended web and mobile synchronization
- Broader market-data integrations

---

## Acknowledgements

Thanks to everyone who contributed to the design, development, testing, supervision, and evaluation of Jisr Platform.

---

## License

This project was developed for academic and portfolio purposes.

A formal open-source license can be added later if the repository is intended for public reuse or redistribution.
