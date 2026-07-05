# Green Care Platform – AI-Powered Plant Care System

Green Care Platform is an AI-powered web platform developed during cooperative training at the Ministry of Environment, Water and Agriculture (MEWA). The platform helps users identify plant species from images, assess plant health based on user inputs, and receive personalized care recommendations using AI and weather-related data.

---

# Project Overview

Many users struggle to care for household plants due to limited knowledge of plant species, incorrect watering habits, and lack of personalized guidance. Green Care Platform addresses this problem by combining computer vision, user input analysis, weather data, and AI-powered recommendations in one simple web-based system.

The platform allows users to upload a plant image, enter basic health-related information, view the predicted plant species, check the plant health status, and receive care recommendations based on the plant type, user inputs, location, temperature, and humidity.

---

# Repository Note

This repository presents the project overview, features, AI workflow, technologies, and screenshots. The source code may be added later after review and cleanup.

---

# Key Features

- User registration and login.
- Plant image upload for species identification.
- AI-based plant species classification.
- Plant health assessment based on user-provided inputs.
- Indoor/outdoor plant category identification.
- Personalized care recommendations.
- Weather-based guidance using location, temperature, and humidity.
- My Plants dashboard to manage and view plant records.
- MySQL database for storing user accounts, plant details, health status, and recommendations.

---

# AI Models

## 1. Plant Species Classification Model

The plant species classification model identifies the plant type from an uploaded image. It is based on MobileNetV2, a lightweight deep learning model suitable for image classification tasks.

The model was trained using the House Plant Species Dataset, which contains around 14,620 images across 47 plant categories. The dataset was split into training, validation, and testing sets. After baseline training and fine-tuning, the validation accuracy improved from 72.75% to 80.30%.

## 2. Plant Health Assessment Model

The plant health assessment model estimates the plant’s health risk level based on structured user inputs such as watering frequency, light exposure, leaf firmness, and humidity.

A Random Forest classifier was trained using a synthetic dataset created to represent different plant stress conditions. The model outputs health risk levels such as healthy, early stress, high risk, and critical.

---

# System Workflow

1. The user uploads a plant image.
2. The user enters plant health information.
3. The image is sent to the FastAPI AI service for plant species prediction.
4. The health inputs are processed to estimate plant stress level.
5. Weather data such as temperature and humidity are retrieved based on the user’s location.
6. The system generates personalized care recommendations.
7. Results are saved in the MySQL database and displayed to the user.

---

# Technologies Used

## Frontend

- HTML
- CSS
- JavaScript

## Backend

- PHP
- FastAPI
- REST APIs

## Database

- MySQL
- XAMPP
- phpMyAdmin

## AI & Machine Learning

- Python
- TensorFlow / Keras
- MobileNetV2
- Scikit-learn
- Random Forest
- Pandas
- NumPy
- Pillow
- Joblib

## External Data

- Weather data
- House Plant Species Dataset

---

# System Architecture

The system consists of four main layers:

1. **Frontend Layer**  
   Provides the user interface for uploading plant images, entering health information, viewing plant records, and receiving recommendations.

2. **Backend Layer**  
   Handles user sessions, database operations, weather data retrieval, and communication with the AI service.

3. **AI Service Layer**  
   Uses FastAPI to run plant species classification and plant health assessment models.

4. **Database Layer**  
   Stores user accounts, plant records, analysis results, and generated recommendations.

---

# Project Scope

## In Scope

- Web-based plant management platform.
- Plant species identification from images.
- User-input health assessment.
- Personalized care recommendations.
- Weather-based recommendation support.
- MySQL data storage.
- Integration between PHP backend and FastAPI AI service.

## Out of Scope

- Advanced plant disease detection.
- IoT-based irrigation control.
- Mobile application development.
- Official integration with MEWA systems.
- Cloud deployment.

---

# Academic Purpose

This project was developed as a cooperative training project to apply artificial intelligence, web development, database management, and system integration skills in a practical solution that supports plant care, sustainability, and environmental awareness.

---

# Future Enhancements

- Add plant disease detection using computer vision.
- Add watering reminders and plant care schedules.
- Deploy the platform on a cloud server.
- Add IoT sensor integration for automatic environmental monitoring.
- Add dashboards to track plant growth and environmental impact.

---

# Author

Ghala Bander Alsuna Allah  
AI Engineer | Artificial Intelligence Graduate

University of Hail
