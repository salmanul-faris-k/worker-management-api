

# 🏗 Worker Management REST API

![Node](https://img.shields.io/badge/Node.js-20-green?logo=node.js)
![Express](https://img.shields.io/badge/Express.js-Backend-black?logo=express)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-green?logo=mongodb)
![Mongoose](https://img.shields.io/badge/Mongoose-ODM-red)
![REST API](https://img.shields.io/badge/API-REST-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)

A production-style **RESTful backend service** for managing construction workers, their daily wages and weekly work-site schedules.

This project digitizes manual labour attendance tracking used in small construction projects and provides a scalable API for dashboard or mobile integration.

---

## 🚀 Features

* Worker CRUD operations
* Weekly site allocation system
* Reset weekly schedules globally
* Default wage handling
* MongoDB persistence
* Clean REST architecture
* Frontend ready API (React / Mobile)

---

## 🧠 Tech Stack

| Layer     | Technology |
| --------- | ---------- |
| Runtime   | Node.js    |
| Framework | Express.js |
| Database  | MongoDB    |
| ODM       | Mongoose   |
| Config    | dotenv     |
| Security  | CORS       |

---

## 📁 Folder Structure

```
worker-management-api
│
├── models
│   └── Worker.js
│
├── routes
│   └── workers.js
│
├── .env
├── index.js
├── package.json
```

---

## ⚙️ Installation

Clone repository

```
git clone https://github.com/YOUR_USERNAME/worker-management-api.git
cd worker-management-api
```

Install dependencies

```
npm install
```

---

## 🔐 Environment Variables

Create `.env` file

```
MONGO_URI=your_mongodb_connection_string
PORT=5000
```

---

## ▶️ Run Server

```
npm start
```

Server runs at

```
http://localhost:5000
```

---

## 📡 API Endpoints

### Get All Workers

```
GET /api/workers
```

---

### Add Worker

```
POST /api/workers
```

Body:

```
{
  "name": "Rahul",
  "dailyRate": 1350,
  "schedule": {
    "S": "",
    "M": "Site A",
    "T": "",
    "W": "",
    "Th": "",
    "F": "",
    "St": ""
  }
}
```

---

### Update Worker

```
PUT /api/workers/:id
```

---

### Delete Worker

```
DELETE /api/workers/:id
```

---

### Reset Weekly Sites

```
PUT /api/workers/reset-sites
```

Resets schedule for all workers.

---

## 📊 Example Response

```
{
  "_id": "65f1a6f3c7d3b2a12c9c1e22",
  "name": "Akshay",
  "dailyRate": 1350,
  "schedule": {
    "S": "",
    "M": "Building Site",
    "T": "",
    "W": "",
    "Th": "",
    "F": "",
    "St": ""
  }
}
```

---

## 🧩 Use Case

Designed for:

* Contractors
* Site supervisors
* Small construction companies
* Labour management dashboards

Replaces paper attendance register with structured digital records.

---

## 🔗 Frontend Integration

This API is designed to connect with React dashboards or mobile apps for real-time worker tracking and wage calculation.

---

## 👨‍💻 Author

**Salmanul Faris K**
MERN Stack Developer

---

## 📜 License

MIT License

---

