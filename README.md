### Full-Stack Fitness Portal

This is a comprehensive Gym Management Application built using the MERN stack. It features a modern, responsive user interface for members to explore workout sessions, calculate fitness metrics, and a functional backend to handle membership inquiries via automated email services.

## 📸 Screenshots

><img width="1883" height="872" alt="Screenshot (26)" src="https://github.com/user-attachments/assets/a6084c70-435a-429c-b11f-5799320248b4" />
<img width="1891" height="881" alt="Screenshot (22)" src="https://github.com/user-attachments/assets/c0bb25cb-e910-404e-bd37-acc1486bc801" />
<img width="1890" height="881" alt="Screenshot (23)" src="https://github.com/user-attachments/assets/8653377c-1c46-40a8-9bdd-61f5c721394b" />
<img width="1889" height="880" alt="Screenshot (24)" src="https://github.com/user-attachments/assets/ad158a6f-620a-484a-9b71-7a53e7a32e40" />

## 🚀 Core Features

* **Interactive BMI Calculator**: A dedicated component allowing users to calculate their Body Mass Index in real-time to track fitness goals.
* **Dynamic Workout Sessions**: Showcases various training programs and bootcamps with a focus on visual storytelling through a gallery and session cards.
* **Membership Pricing**: Transparent tiered pricing plans to help users choose the best fitness package for their needs.
* **Automated Contact System**: A functional contact form integrated with a **Node.js/Nodemailer** backend to send inquiries directly to gym management.
* **Responsive Navigation**: A sleek, mobile-friendly Navbar and Footer ensuring a seamless experience across all devices.

## 🛠 Tech Stack

* **Frontend**: React.js, CSS3 (Custom animations and layouts).
* **Backend**: Node.js, Express.js.
* **Email Service**: Nodemailer (via `sendEmail.js` utility) for handling contact form submissions.
* **Deployment**: Structured for easy deployment on platforms like Vercel (Frontend) and Render (Backend).

## 🏗 Key Implementation Details

### 1. Backend Inquiry Handling

The application uses a custom utility `sendEmail.js` located in the backend. When a user submits the `Contact.jsx` form, the backend processes the request and uses **Nodemailer** to dispatch an email, ensuring gym owners never miss a lead.

### 2. Component-Based Architecture

The frontend is highly modular. Components like `Gallery.jsx` and `WorkoutSessions.jsx` are designed to be reusable and easily updatable with new gym content or promotional events.

### 3. Integrated BMI Logic

The `BMICalculator.jsx` provides instant feedback to users. I implemented the mathematical logic within the React state to provide an interactive "health-check" tool directly on the landing page.

## 📁 Project Structure

```text
gym-management/
├── backend/
│   ├── utils/
│   │   └── sendEmail.js    # Nodemailer configuration
│   ├── app.js              # Express server & API routes
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/     # UI Components (Hero, Navbar, BMI, etc.)
│   │   ├── App.jsx         # Main Application logic
│   │   └── App.css         # Global styling
│   └── package.json
└── README.md

```

## 🛠 Installation & Setup

1. **Clone the Repository**
```bash
git clone https://github.com/yourusername/eliteedge-gym.git

```


2. **Backend Setup**
```bash
cd backend
npm install
# Create a .env file and add your SMTP credentials (EMAIL, PASSWORD)
npm start

```


3. **Frontend Setup**
```bash
cd frontend
npm install
npm run dev

```
