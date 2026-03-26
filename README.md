# Vi-Notes – User Authentication Module

Vi-Notes is an authenticity verification platform designed to distinguish genuine human-written content from AI-generated or AI-assisted text. The system focuses on analyzing writing behavior alongside statistical and linguistic characteristics of text.

This contribution implements the **User Login and Registration feature**, which serves as the foundation for associating writing sessions with individual users.

---

## Feature Implemented

### User Login and Registration

Implemented basic user authentication to ensure that each writing session can be linked to a specific user.

* Users can sign up using email and password
* Users can log in using the same credentials
* Duplicate user validation is handled
* Invalid login attempts are handled
* Successful login redirects user to a basic editor page

Advanced features such as roles, password reset, and authentication tokens are not included at this stage.

---

## Tech Stack

### Frontend

* React (TypeScript)
* Vite
* React Router DOM

### Backend

* Node.js
* Express.js
* TypeScript

### Database

* MongoDB Atlas

---

## Project Structure

```
vi-notes/
├── client/        # Frontend (React + Vite)
├── server/        # Backend (Node + Express)
└── README.md
```

---

## Setup Instructions

### 1. Clone the Repository

```
git clone https://github.com/Nencypatel21/vi-notes.git
cd vi-notes
```

---

## Backend Setup

```
cd server
npm install
```

Create a `.env` file inside the `server` directory:
```
MONGO_URL=your_mongodb_connection_string_here
```

Run the backend server:
```
npm run dev
```

The backend will run on:
```
http://localhost:5000
```

---

## Frontend Setup

```
cd client
npm install
```

Create a `.env` file inside the `client` directory:
```
VITE_API_URL=http://localhost:5000/api
```

Run the frontend:
```
npm run dev
```

The frontend will run on:
```
http://localhost:5173
```

---

## Application Flow

```
Home → Signup → Login → Editor
```

* Users register using email and password
* Users log in with registered credentials
* After login, users are redirected to a basic editor page

---

## Contribution Scope

This contribution includes:

* Implementation of authentication APIs (register and login)
* Integration with MongoDB Atlas
* Frontend forms for signup and login
* API integration between frontend and backend
* Basic navigation flow

This serves as a foundational step for future features such as writing behavior analysis and authenticity verification.

---

## Important Notes

* `.env` files are not included in the repository for security reasons
* A valid MongoDB connection string is required to run the backend
* Backend server must be running before starting the frontend

---

## Author

PATEL NENCY DASHARATHBHAI
---

## License

This project is licensed under the MIT License.
