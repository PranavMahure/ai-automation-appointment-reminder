# Appointment Reminder System

A full-stack Appointment Reminder System built using React, Node.js, Express, and SQLite. This application allows users to create appointments, store them in a database, view them through a dashboard, and automatically send confirmation and reminder messages.

## Features

* Create appointments with customer name, phone number, and appointment time
* Store appointment data in a SQLite database
* Live dashboard displaying all appointments
* Automatic appointment confirmation messages
* Automated reminder system for upcoming appointments
* Mock SMS service included for testing
* Easily replaceable with Twilio SMS or WhatsApp API integration

## Tech Stack

### Frontend

* React
* Vite
* Axios

### Backend

* Node.js
* Express.js

### Database

* SQLite

### Automation

* Node-Cron

## Project Structure

```text
appointment-reminder-system/
├── backend/
│   ├── routes/
│   ├── database.js
│   ├── scheduler.js
│   ├── smsService.js
│   └── server.js
│
├── frontend/
│   ├── src/
│   ├── index.html
│   ├── vite.config.js
│   └── package.json
│
└── README.md
```

## Installation

### Clone Repository

```bash
git clone <repository-url>
cd appointment-reminder-system
```

### Backend Setup

```bash
cd backend
npm install
npm run dev
```

Backend runs on:

```text
http://localhost:5000
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Frontend runs on:

```text
http://localhost:5173
```

## Application Workflow

1. User enters customer details and appointment time.
2. Appointment is saved to the SQLite database.
3. Confirmation message is triggered.
4. Appointment appears on the dashboard.
5. Background scheduler checks appointments every minute.
6. Reminder messages are sent for appointments occurring within one hour.

## SMS/WhatsApp Integration

The current implementation uses a mock messaging service for demonstration purposes:

```javascript
console.log("MOCK SMS =>", phone, message);
```

To send real messages, replace the mock implementation with:

* Twilio SMS API
* Twilio WhatsApp Sandbox
* WhatsApp Cloud API

## Future Improvements

* Twilio WhatsApp Integration
* Appointment Editing and Deletion
* Form Validation
* Authentication and User Roles
* Email Notifications
* Deployment on Render/Vercel
* Docker Support

## Author

Pranav

## Time Taken

Approximately 4–6 hours including design, development, testing, and documentation.

## License

This project was developed as part of an AI Automation Developer Practical Assessment.
