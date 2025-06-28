# Full-Stack GraphQL App (Node.js + React)

This project is a full-stack implementation of a **GraphQL-powered blog and authentication system** using **Node.js (Express)**, **MongoDB**, and **ReactJS**. It demonstrates GraphQL query/mutation handling, file upload via resolvers, JWT authentication, and a modular UI.

---

## 🔗 Repository

**GitHub:** [graphql](https://github.com/ajayvishwakarma457/graphql)

---

## 🚀 Features

### Backend (GraphQL + Node.js)
- 📡 GraphQL API via `express-graphql`
- 🧩 Modular resolvers and schema
- 🔐 JWT authentication middleware
- 🖼️ Image/file uploads using custom resolvers
- 🧱 Mongoose models for User and Post

### Frontend (React)
- 🔐 Login/Signup with persistent JWT storage
- 📝 Create & view posts using GraphQL
- 📸 Upload profile/post images
- 💬 Feed with pagination
- 🚦 Client-side routing and auth flow

---

## 🧱 Project Structure

graphql/
├── backend/
│ ├── graphql/
│ │ ├── resolvers.js # Logic for GraphQL queries/mutations
│ │ └── schema.js # SDL-based type definitions
│ ├── controllers/ # Optional REST controllers or shared logic
│ ├── middleware/ # JWT Auth middleware
│ ├── models/ # Mongoose models (User, Post)
│ ├── util/ # File helpers (e.g., image uploads)
│ ├── images/ # Uploaded files
│ ├── app.js # Express app + GraphQL middleware
│ └── .env # Environment variables
│
├── frontend/
│ ├── public/
│ ├── src/
│ │ ├── components/ # Reusable UI elements
│ │ ├── pages/ # Feed and Auth routes
│ │ ├── util/ # Validators and helpers
│ │ └── App.js / index.js # Main app logic
│ ├── notes/ # Dev notes or scratch files
│ └── package.json


---

## 🛠 Technologies Used

### Backend:
- Node.js
- Express.js
- MongoDB + Mongoose
- GraphQL (`express-graphql`)
- JWT (Authentication)
- Multer (Image upload)

### Frontend:
- ReactJS
- React Router
- Axios
- Apollo Client (optional, or raw fetch)
- CSS Modules

---

## ⚙️ Getting Started

### 1. Setup MongoDB

You need a MongoDB instance (local or Atlas). Add your connection string in:

backend/.env

```env
MONGODB_URI=mongodb://localhost:27017/graphql-blog
JWT_SECRET=your-secret-key

Run Backend
  cd backend
  npm install
  node app.js

GraphQL Playground available at:
http://localhost:8080/graphql

Run Frontend
  cd frontend
  npm install
  npm start

## 📬 Contact
  **Author:** Ajay M Vishwakarma  
  **Email:** ajayvishwakarma457@gmail.com

📄 License
  This repository is licensed under the MIT License.
  See the LICENSE file for details.


