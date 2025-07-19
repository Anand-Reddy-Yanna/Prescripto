# Prescripto 🩺

**Prescripto** is a complete healthcare backend platform built with Node.js, Express, and MongoDB. It supports user registration, appointment scheduling, digital prescriptions, and Razorpay integration for payments. This project streamlines patient-doctor interactions and is ideal for clinics or digital health services.

---

## 🌟 Features

- 🔐 User Authentication (JWT based)
- 👨‍⚕️ Doctor Profile Management (CRUD)
- 📅 Appointment Booking and Management
- 💊 Prescription System for Doctors
- 💳 Razorpay Payment Integration
- 📁 Modular and Scalable Code Structure
- 📦 Environment Configuration via `.env`

---

## 🛠️ Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MongoDB with Mongoose
- **Authentication**: JWT
- **Validation**: JOI
- **Payments**: Razorpay
- **Logging**: Morgan

---

## 📁 Folder Structure

```
Prescripto/
├── config/          # Configuration files
├── controllers/     # Route logic and controller methods
├── middlewares/     # Auth, validation, error handling
├── models/          # Mongoose schemas
├── routes/          # API route definitions
├── utils/           # Helper utilities
├── server.js        # Entry point
└── .env             # Environment variables
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Anand-Reddy-Yanna/Prescripto.git
cd Prescripto
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Setup Environment Variables

Create a `.env` file in the root directory and add the following:

```env
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
PORT=5000
```

### 4. Run the Development Server

```bash
npm start
```

The backend will start on `http://localhost:5000`.

---

## 🔌 API Endpoints

| Method | Endpoint              | Description                 |
|--------|-----------------------|-----------------------------|
| POST   | `/api/auth/register`  | Register a new user         |
| POST   | `/api/auth/login`     | Login existing user         |
| GET    | `/api/doctors`        | List all doctors            |
| POST   | `/api/doctors`        | Add a new doctor            |
| POST   | `/api/appointments`   | Book an appointment         |
| POST   | `/api/prescriptions`  | Create prescription         |
| POST   | `/api/payments`       | Handle payments via Razorpay|

> Note: Use proper JWT tokens in headers for protected routes.

---

## 📦 Sample `.env` File

```env
MONGODB_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/prescripto
JWT_SECRET=mySuperSecretToken
RAZORPAY_KEY_ID=yourRazorpayKeyId
RAZORPAY_KEY_SECRET=yourRazorpaySecret
PORT=5000
```

---

## 🧠 Future Improvements

- Add Swagger API Docs
- Email/SMS Notifications
- Admin Dashboard
- Real-Time Appointment Status
- Frontend Integration (React or Angular)

---

## 👨‍💻 Author

**Anand Reddy Yanna**  
GitHub: [@Anand-Reddy-Yanna](https://github.com/Anand-Reddy-Yanna)
