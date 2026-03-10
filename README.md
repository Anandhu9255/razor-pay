# 💳 Razorpay Payment Gateway Integration

A clean and functional implementation of the Razorpay payment ecosystem. This project serves as a robust boilerplate for integrating secure, real-time payments into any web application, ensuring data integrity through server-side verification.

## 📋 Table of Contents
- [Project Overview](#-project-overview)
- [Payment Flow](#-payment-flow)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [Installation & Setup](#-installation--setup)
- [Security Implementation](#-security-implementation)
- [License](#-license)

---

## 🌟 Project Overview
This repository provides a complete end-to-end flow for processing online payments. It handles everything from initiating an order via the backend to processing the payment UI and verifying the payment signature to prevent fraud.

## 🔄 Payment Flow
1. **Order Creation:** The frontend sends a request to the backend to create a unique `order_id`.
2. **Checkout:** The Razorpay Checkout script opens a secure modal for the user to enter payment details.
3. **Verification:** Once payment is successful, Razorpay returns a signature which is verified on the backend using the `razorpay_signature` and `HmacSHA256` algorithm.

## ✨ Key Features
- **Secure Transactions:** Backend signature validation to confirm payment authenticity.
- **Dynamic Pricing:** Support for custom amounts and currency configurations.
- **Modern UI:** A clean, user-friendly interface for triggering the payment modal.
- **Environment Safety:** Centralized configuration for API keys and secrets using environment variables.
- **Real-time Feedback:** Instant success or failure alerts for the user post-transaction.

## 🛠 Tech Stack
- **Frontend:** HTML5, CSS3, JavaScript (Vanilla/React)
- **Backend:** Node.js, Express.js
- **Payment Gateway:** Razorpay API
- **Utilities:** Crypto (for signature verification), Dotenv

---

## ⚙️ Installation & Setup

### Prerequisites
- Node.js installed
- A Razorpay Dashboard account (Test or Live mode)
- API Key ID and Key Secret from Razorpay

### 1. Clone the Repository
```bash
git clone [https://github.com/Anandhu9255/razor-pay.git](https://github.com/Anandhu9255/razor-pay.git)
cd razor-pay

### 2. Install Dependencies
```bash
npm install

### 3. Environment Configuration
Create a .env file in the root directory and add your credentials:

Code snippet
RAZORPAY_KEY_ID=your_key_id_here
RAZORPAY_KEY_SECRET=your_key_secret_here
PORT=5000

### 4. Run the Application
```bash
# Start the server
npm start
Access the application at http://localhost:5000.
