# Lung Capacity Enhancer

This project consists of an Arduino code for the Lung Capacity Enhancer device and a web application with separate frontend and backend.

## Table of Contents
- [Problem Statement](#problem-statement)
- [About Device](#about-device)
- [Arduino Code (Lung_Capacity_Enhancer)](#arduino-code-lung_capacity_enhancer)
- [Installation (Website)](#installation-Website)
- [Web Application (Website)](#web-application-website)
  - [Frontend](#frontend)
  - [Backend](#backend)
- [Usage](#usage)


## Problem Statement
In India, pediatric respiratory care poses significant challenges, encompassing healthcare, emotional well-being, and practical considerations, and these challenges have intensified further following the COVID-19 pandemic. Traditional methods lack sufficient user engagement, often resulting in non-compliance among young patients facing respiratory challenges. The current landscape also faces issues of cost-effectiveness, hindering widespread access to effective treatment. Hygiene concerns in healthcare settings further amplify the need for innovative solutions that prioritize cleanliness and portability. Emotional support for pediatric patients during respiratory treatments is often overlooked. Considering these multifaceted challenges, there is a pressing need for a comprehensive and user-centric solution that not only addresses clinical efficacy but also factors in cost-effectiveness, hygiene standards, and emotional well-being. A portable device that combines sensor technology, gamification for enhanced user engagement, cost-effective components, and a focus on hygiene would significantly contribute to overcoming the existing barriers in pediatric respiratory care in India.

## About Device
A standalone device with dedicated software designed as an interactive game for children and adults to enhance their lung capacity, especially those suffering from respiratory issues.
![Device Image](images/Device.png)
![Device Image](images/HighLevelDesign.png)

## Arduino Code (Lung_Capacity_Enhancer)
This folder contains the Arduino code for the Lung Capacity Enhancer device.

## Installation(Website)
Provide step-by-step instructions on how to install and set up both the Arduino code and the web application.
1. Clone the repository:
   
   git clone https://github.com/Kunal-Wagh282/Lung_Capacity_Enhancer-GDSC-Repo-
2. Navigate to the Website directory:
   
       cd Website

## Web Application (Website)
The web application consists of two parts: frontend and backend.

## Frontend
This folder contains the frontend code for the Lung Capacity Enhancer web application.
### Frontend Features

#### Registration Page
- **User Registration**: Users can register with their username, first name, last name, date of birth, and password. The minimum age requirement for registration is 5 years old.

#### Login Page
- **User Login**: Registered users can log in with their username and password, and retrieve their profile information.

#### Dashboard
- **Profile Management**: Users can add, delete, and view their profiles. Each profile has a name and date of birth.
- **Bluetooth Connection**: Users can establish a Bluetooth connection with the device.
- **Real-time Graph**: Users can view real-time graph data while blowing into the device.

#### History Page
- **View Past Data**: Users can view past history data in the form of graphs.

#### Analysis Page
- **Generate Analysis**: Users can select a range of dates and view analysis reports.


### Prerequisites
- Node.js installed on your computer
- Vite installed on your computer

### Installation
1. Navigate to the `frontend` directory:
   
       cd frontend

2. Install dependencies:

       npm install

### Usage
   To run the development server, use the following command:

    npm run dev

## Backend
This folder contains the backend code for the Lung Capacity Enhancer web application.
This is a Django-based backend API that provides various functionalities such as user registration, login, profile management, graph data storage and retrieval, and report generation.

### Backend Features

- **User Registration**: Users can register with their username, first name, last name, date of birth, and password. The minimum age requirement for registration is 5 years old.
- **User Login**: Registered users can log in with their username and password, and retrieve their profile information.
- **Profile Management**: Users can add, delete, and view their profiles. Each profile has a name and date of birth.
- **Graph Data Storage**: Users can save graph data, including time and volume arrays, for their profiles. The total volume (area under the curve) is calculated and stored.
- **Graph Data Retrieval**: Users can retrieve their graph data for a specific date and profile.
- **Report Generation**: Users can generate reports containing their graph data within a specified date range for a particular profile.

### Installation
   
1. Navigate to the project directory:
   
       cd backend
   

2. Create a virtual environment (optional but recommended):
   
       python -m venv env
       source env/bin/activate  # On Windows, use `env\Scripts\activate`
   

3. Install the required dependencies:
   
       pip install -r requirements.txt
   

4. Set up the Django project:
   
       python manage.py migrate
   

### Usage

1. Start the Django development server:
   
       python manage.py runserver
   

2. The API endpoints can be accessed at `http://localhost:8000/api/`. You can use tools like Postman or cURL to interact with the API.

3. Refer to the `api/urls.py` file for the available endpoints and their corresponding views in `api/views.py`.

### API Endpoints

- `POST /api/register/`: Register a new user.
- `POST /api/login/`: Log in an existing user.
- `POST /api/add-profile/`: Add a new profile for a user.
- `POST /api/del-profile/`: Delete a profile for a user.
- `POST /api/graph-data/`: Save graph data for a user's profile.
- `POST /api/get-graph-data/`: Retrieve graph data for a user's profile on a specific date.
- `POST /api/generate-report/`: Generate a report containing graph data for a user's profile within a specified date range.





## Usage
Provide examples and usage instructions for the Lung Capacity Enhancer device and the web application.

