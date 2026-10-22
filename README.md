# Celestius – Event Registration Backend

## 1. Project Description

A simple backend API for managing registrations for the Backend Development Workshop using Python, Flask, and SQLite.

## 2. Event Details

- **Event:** Backend Development Workshop
- **Date:** 20 October 2026
- **Capacity:** 50 participants

## 3. Technologies Used

- Python
- Flask
- SQLite
- REST API

## 4. Features

- Register participants using their name and email.
- Store registration details in an SQLite database.
- View all registrations.
- Retrieve an individual registration by ID.
- Reject duplicate email addresses.
- Validate required fields.
- Limit registrations to 50 participants.

## 5. Setup Instructions

### Step 1: Install Flask

```bash
pip install flask
```

### Step 2: Run the Application

```bash
python app.py
```

The server runs at: `http://127.0.0.1:5000`

## 6. API Endpoints

| HTTP Method | Endpoint | Description |
|---|---|---|
| GET | `/` | Check server status |
| POST | `/register` | Register a participant |
| GET | `/registrations` | View all registrations |
| GET | `/registrations/<id>` | View a registration by ID |

## 7. Example Registration Request

Send a POST request to `/register` with the following JSON data:

```json
{
  "name": "Priya",
  "email": "priya2026@example.com"
}
```

## 8. Database

SQLite stores participant details in `registrations.db`. The database table is created automatically when the application starts.

## 9. Author

NAME : Praisy Evangeline D
