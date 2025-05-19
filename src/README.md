# Mergington High School Activities

A web application that allows students to view and sign up for extracurricular activities at Mergington High School, with additional teacher management features.

## Features

### For Students
- View all available extracurricular activities
- Filter activities by category (Sports, Arts, Academic, Community, Technology)
- Filter activities by day (Monday through Sunday)
- Filter activities by time (Before School, After School, Weekend)
- Search activities by name or description
- Sign up for activities (through teacher assistance)

### For Teachers
- Secure login/authentication system
- Manage student activity registrations
- Sign up students for activities
- Remove students from activities

## Technology Stack

- Frontend: HTML, CSS, JavaScript
- Backend: FastAPI (Python)
- Database: MongoDB (in-memory during development)

## API Endpoints

- `GET /activities` - Get all activities with optional day and time filters
- `GET /activities/days` - Get all available days that have scheduled activities
- `POST /activities/{activity_name}/signup` - Register a student for an activity
- `POST /activities/{activity_name}/unregister` - Remove a student from an activity
- `POST /auth/login` - Teacher login
- `GET /auth/check-session` - Validate teacher session

## Development Guide

For detailed setup and development instructions, please refer to our [Development Guide](../docs/how-to-develop.md).
