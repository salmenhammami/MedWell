# MedWell

A modern healthcare and wellness platform designed to simplify medical appointments, patient record management, and daily health tracking.

## Overview

**MedWell** is built to improve the digital healthcare experience for both patients and providers. It offers a clean, centralized system to schedule medical consultations, manage health profiles, track vitals, and maintain organized treatment records securely.

## Key Features

* **Appointment Scheduling:** Book, reschedule, and manage doctor appointments with real-time status updates.
* **Patient & Medical Records:** Centralized dashboard for storing patient history, prescriptions, and health metrics.
* **User & Role Management:** Secure authorization tiers for patients, healthcare providers, and administrative staff.
* **Health & Vitals Tracking:** Interactive interface for logging and viewing health trends over time.

## Tech Stack

* **Backend:** PHP (RESTful API Architecture)
* **Frontend:** React (Vite)
* **Database:** MySQL
* **Authentication:** Session-based / Role-Based Access Control (RBAC)

## Getting Started

### Prerequisites
* PHP 8.0+
* MySQL / XAMPP / WAMP
* Node.js & npm

### Quick Setup

```bash
# Clone the repository
git clone https://github.com/HammamiSalmen/MedWell.git
cd MedWell

# Backend Setup
cd backend
# Run locally using PHP built-in server (or configure via XAMPP/Apache)
php -S localhost:8000

# Frontend Setup (in a new terminal)
cd ../frontend
npm install
npm run dev
