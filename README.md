# Recreation of TN Startup Website

## Overview

This project is a **recreation of the TN Startup Website**, built as a full-stack application. It features a **React.js** frontend styled with **Tailwind CSS**, and a **Node.js** backend connected to a **MongoDB** database. The application offers a responsive design, dynamic content management, and a scalable backend to manage startup-related data.

---

## Features

- **Home Page**: A modern and responsive landing page showcasing startup initiatives.
- **Dynamic Data**: Startups, events, and updates are dynamically fetched from the backend.
- **Admin Panel**: CRUD operations for managing startup details and user data.
- **Responsive Design**: Fully optimized for mobile, tablet, and desktop views.
- **Secure API**: Authentication and validation for backend routes.

---

## Tech Stack

### Frontend
- **React.js**
- **Tailwind CSS**
- **Axios** for API communication

### Backend
- **Node.js**
- **Express.js**

### Database
- **MongoDB** (cloud or local)

---

## Installation and Setup

### Prerequisites
1. **Node.js** (v16.x or above)
2. **MongoDB** (local or MongoDB Atlas)
3. **npm** or **yarn**

### Clone the Repository
```bash
git clone https://github.com/your-repo/TN-Startup-Website.git
cd TN-Startup-Website
```

---

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the `backend` directory and add the following variables:
   ```env
   PORT=5000
   MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/<dbname>?retryWrites=true&w=majority
   ```
4. Start the backend server:
   ```bash
   npm start
   ```

---

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd ../frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the frontend development server:
   ```bash
   npm start
   ```

---

## Project Structure

### Frontend
```
frontend/
├── src/
│   ├── components/
│   ├── pages/
│   ├── services/
│   └── App.js
└── package.json
```

### Backend
```
backend/
├── routes/
├── controllers/
├── models/
├── config/
├── server.js
└── package.json
```

---

## API Endpoints

### Base URL: `http://localhost:5000/api`

| Method | Endpoint            | Description                          |
|--------|---------------------|--------------------------------------|
| GET    | `/startups`         | Fetch all startup data               |
| POST   | `/startups`         | Add a new startup                   |
| PUT    | `/startups/:id`     | Update a startup by ID               |
| DELETE | `/startups/:id`     | Delete a startup by ID               |
| GET    | `/events`           | Fetch all events                    |
| POST   | `/events`           | Add a new event                     |

---

## Scripts

### Backend
- Start the backend server:
  ```bash
  npm start
  ```

### Frontend
- Start the React development server:
  ```bash
  npm start
  ```

---

## Environment Variables

| Variable      | Description                                       |
|---------------|---------------------------------------------------|
| `PORT`        | Port number for the backend server               |
| `MONGO_URI`   | Connection string for MongoDB database           |

---

## Future Enhancements

- Add user authentication using **JWT** for admin and user roles.
- Implement **pagination** for handling large datasets.
- Include **analytics dashboards** for startup growth tracking.
- Add **chat support** for startups and mentors.

---

## Troubleshooting

- **Frontend not connecting to backend**: Ensure the backend server is running and the correct API URL is used in `frontend/src/services/axiosInstance.js`.
- **Database connection issues**: Verify the `MONGO_URI` value in the `.env` file.
- **Styling issues**: Check the Tailwind CSS setup in `tailwind.config.js`.

---

## Contributors

- **Gokul Nath S** - Developer
- Contributions are welcome! Submit a pull request.

---
