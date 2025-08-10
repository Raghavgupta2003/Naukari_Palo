Alright Raghav — here’s your **complete `README.md`** with the environment variables section safely updated so no sensitive data is leaked.

---

````markdown
# MERN Job Seeking Web App

A job-seeking platform built with the **MERN stack** (MongoDB, Express, React, Node.js) that allows users to post, apply for, and view job listings.

---

## 📂 Project Setup

### 1️⃣ Clone Repository
First, clone the repository to your local machine:

```bash
git clone <your-github-repo-url>
````

Navigate into the project folder:

```bash
cd <repo-folder-name>
```

---

## ⚙️ Backend Setup

### 2️⃣ Create Config Folder and Environment File

Inside the `backend` folder, create a folder named `config` and a file `config.env`:

```
backend/
└── config/
    └── config.env
```

Paste the following environment variables into `config.env`:

```env
MONGO_URI=your_mongodb_connection_string
PORT=4000
CLOUDINARY_CLIENT_NAME=your_cloudinary_cloud_name
CLOUDINARY_CLIENT_API=your_cloudinary_api_key
CLOUDINARY_CLIENT_SECRET=your_cloudinary_api_secret
FRONTEND_URL=http://localhost:5173
JWT_SECRET_KEY=your_jwt_secret
JWT_EXPIRE=7d
COOKIE_EXPIRE=5
```

---

### 📌 How to Get These Values:

* **MONGO\_URI** →
  Get this from your MongoDB connection.

  * For local MongoDB:
    `mongodb://localhost:27017/<your_database_name>`
  * For MongoDB Atlas: Copy the connection string from the **"Connect"** section in your MongoDB Atlas dashboard.

* **PORT** →
  The backend server port. Common values are `4000` or `5000`.

* **CLOUDINARY\_CLIENT\_NAME, CLOUDINARY\_CLIENT\_API, CLOUDINARY\_CLIENT\_SECRET** →
  Sign up on [Cloudinary](https://cloudinary.com/), go to the **Dashboard**, and copy these values.

* **FRONTEND\_URL** →
  URL where your frontend runs during development.

  * For local development with Vite, this is usually `http://localhost:5173`.

* **JWT\_SECRET\_KEY** →
  Any random secret string used to sign JSON Web Tokens.

  * Example: generate one with [randomkeygen.com](https://randomkeygen.com/).

* **JWT\_EXPIRE** →
  Token expiration time. Example: `7d` for 7 days.

* **COOKIE\_EXPIRE** →
  Number of days before cookies expire.

> ⚠️ **Important:** Never commit `.env` files to GitHub. Add `config.env` to your `.gitignore` file.

---

### 3️⃣ Install Backend Dependencies

Navigate to the backend folder:

```bash
cd backend
npm install
```

---

### 4️⃣ Start Backend Server

```bash
npm start
```

> The backend will run on **[http://localhost:4000](http://localhost:4000)** by default.

---

## 💻 Frontend Setup

### 5️⃣ Install Frontend Dependencies

Open a new terminal, navigate to the `frontend` folder:

```bash
cd frontend
npm install
```

---

### 6️⃣ Start Frontend Development Server

```bash
npm run dev
```

> The frontend will run on **[http://localhost:5173](http://localhost:5173)** by default.

---

## 📦 Scripts

* **Backend**

  * `npm start` → Starts server with Node
  * `npm run dev` → Starts server with Nodemon (for development)

* **Frontend**

  * `npm run dev` → Starts Vite development server

---

## 🛠 Tech Stack

* **Frontend:** React, Vite
* **Backend:** Node.js, Express.js
* **Database:** MongoDB
* **Other Tools:** Cloudinary, JWT, Bcrypt, CORS, Dotenv

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Raghav Gupta**

