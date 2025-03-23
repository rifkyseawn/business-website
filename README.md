# Business Website Template

This template is a fully functional business website built with **React 18** (using **TypeScript 4**), **Material UI 5**, **Django 4**, and **Django REST Framework 3**.

## Table of Contents
- [Requirements](#requirements)
- [Setup Instructions](#setup-instructions)
- [Launch Application](#launch-application)
- [Quality Assurance](#quality-assurance)
- [Data Management](#data-management)
- [Customization Guide](#customization-guide)
- [License](#license)

## Requirements

Essential components to install:

1. [Python 3.8-3.11](https://www.python.org/downloads/)  
   *Required for Django 4.2.4 - [Compatibility Guide](https://django.readthedocs.io/en/stable/faq/install.html)*
2. [Node.js LTS](https://nodejs.org/en/)
3. [VS Code](https://code.visualstudio.com/) (Recommended IDE)

## Setup Instructions

### Backend Configuration

#### 1. Initialize Virtual Environment

Open your terminal, navigate to the backend folder, and run:

```bash
cd backend
python -m venv venv
```

#### 2. Activate Environment

On macOS:

```bash
source venv/bin/activate
```

On Windows:

```bash
venv\scripts\activate
```

#### 3. Install Dependencies

Within the backend directory, install the required packages:

```bash
pip install -r requirements.txt
```

#### 4. Database Setup

Execute the following commands to apply migrations:

```bash
python manage.py makemigrations
python manage.py migrate
```

#### 5. Admin Credentials

To access the Django admin panel, create an admin user:

```bash
python manage.py createsuperuser
```

Provide a username, email, and password when prompted.

### Frontend Configuration

#### 1. Install Packages

From the project root, navigate to the frontend folder and install the dependencies:

```bash
cd frontend
npm install
```

## Launch Application

To run the full application, you need both the backend and frontend servers running concurrently.

### 1. Start Backend Server

From the backend folder, run:

```bash
python manage.py runserver
```

### 2. Launch Frontend

From the frontend folder, run:

```bash
npm start
```

Once both servers are running, open your browser and navigate to http://localhost:3000/ to view the application.

## Data Management

You can add data to the application through Django Admin.
Open your browser and visit http://127.0.0.1:8000/admin to log in with your admin credentials and manage your data.
