# hall-booking-system

This repository contains a full-stack Hall Booking application developed as part of the Ascentech Internship Interview Exercise.

The project demonstrates the use of a modern web stack with proper separation of concerns, secure configuration handling, and ORM-based database operations.

🚀 Tech Stack
Frontend
React.js
Axios for API communication
Backend
Python (Django)
Django REST Framework
Django ORM
Database
PostgreSQL (self-hosted)
✨ Features
Create a new hall booking
View list of existing bookings
Update an existing booking (via API)
Delete a booking (via API)
REST-based architecture
All CRUD operations handled using ORM
Secure configuration using environment variables
🔐 Configuration & Security
⚠️ No secrets, credentials, URLs, or database information are hardcoded in this repository.

All sensitive values are injected at runtime using operating system environment variables, which is a standard industry best practice.

Required Environment Variables
The following environment variables must be set outside the project:

DJANGO_SECRET_KEY
DB_NAME
DB_USER
DB_PASSWORD
DB_HOST
DB_PORT
REACT_APP_API_URL
An .env.example file is provided only as a reference and does not contain any actual values.

🛠️ Backend Setup (Django)
cd backend
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
Backend will run at:

http://localhost:8000
API endpoint:

http://localhost:8000/api/bookings/
🎨 Frontend Setup (React)
cd frontend
npm install
npm start
Frontend will run at:

http://localhost:3000
🧪 Usage
Start PostgreSQL and ensure the database exists
Start the Django backend
Start the React frontend
Create a booking using the UI
View bookings rendered from the backend API
📁 Project Structure
hall-booking-project/
├── backend/    # Django REST API
├── frontend/   # React application
├── .env.example
└── README.md
🎥 Demo Video
A Loom video explaining:

Project architecture
Environment configuration
Backend ORM usage
Frontend-backend integration
is included as part of the submission.

📌 Notes
All database operations are performed using ORM
No raw SQL queries are used
No credentials are committed to the repository
Project is ready for local development and evaluation
👤 Author
Developed by Akanksha Kamra Ascentech Internship Interview Submission
