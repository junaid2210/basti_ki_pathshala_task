# 🚀 Internship Task – Volunteer/Intern Registration Backend

A simple Node.js + Express + MongoDB backend for registering users as **volunteers** or **interns**, and for viewing the list of all registered users.

---

## 🛠 Tech Stack

- Node.js  
- Express.js  
- MongoDB (via Mongoose)  
- express-validator  
- dotenv  

---

## 📦 Setup Instructions

1. **Clone the repo**
```
git clone https://github.com/<your-username>/internship-backend.git
cd internship-backend
```

2. **Install dependencies**
```
npm install
```

3. **Create a `.env` file** in the root directory:
```
MONGODB_URI=your_mongodb_connection_string
```

4. **Start the server**
```
node index.js
```

Server will run at:  
`http://localhost:3000`

---

## 📡 API Endpoints

### ➕ POST `/register`

Registers a new user.

**Request Body**
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "phone": "9999999999",
  "role": "intern"
}
```

- `role` must be `"intern"` or `"volunteer"`

---

### 📋 GET `/users`

Returns all registered users in JSON format.

---

## 📁 Project Structure

```
.
├── models/
│   └── User.js
├── .env             # Environment variables (not committed)
├── .gitignore
├── index.js         # Main server code
├── package.json
└── README.md
```

---

## ✅ Notes

- The `.env` file is excluded via `.gitignore`
- Test endpoints using Postman or Thunder Client
- Project kept minimal and clean for internship evaluation
