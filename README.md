# VEDA AURA - Luxury Natural Beauty & Skincare

A complete, production-ready full-stack e-commerce application for VEDA AURA, featuring a premium minimal aesthetic and robust cloud integration.

## 🌿 Brand Identity
- **Name:** VEDA AURA
- **Niche:** Luxury natural skincare
- **Aesthetic:** Minimalist botanical, premium beige/off-white palette, Playfair Display & Inter typography.

## 🛠 Tech Stack
- **Frontend:** React (Vite) + Tailwind CSS + Framer Motion
- **Backend:** Node.js + Express
- **Database:** MongoDB (Mongoose)
- **State Management:** Zustand (with Persistence)
- **Auth:** JWT + OTP via Twilio Verify API
- **Payments:** Razorpay
- **Media:** Cloudinary (Multer handling)
- **Notifications:** Twilio (WhatsApp & SMS)
- **Email:** Nodemailer (SMTP)
- **Charts:** Chart.js

## 📁 Folder Structure
- `/client`: React (Vite) frontend with Tailwind 4.
- `/server`: Express backend with Mongoose models and controllers.
- `/seed`: Scripts for populating the database with brand-appropriate products.

## 🚀 Setup Instructions

### 1. Variables
Create a `.env` file in the `/server` folder using the structure below:
```env
PORT=5000
MONGO_URI=your_mongodb_atlas_uri
JWT_SECRET=your_jwt_secret

RAZORPAY_KEY_ID=your_key_id
RAZORPAY_KEY_SECRET=your_key_secret

TWILIO_ACCOUNT_SID=your_sid
TWILIO_AUTH_TOKEN=your_token
TWILIO_VERIFY_SERVICE_SID=your_verify_sid
TWILIO_WHATSAPP_FROM=your_number

CLOUDINARY_CLOUD_NAME=your_name
CLOUDINARY_API_KEY=your_key
CLOUDINARY_API_SECRET=your_secret

SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your_email
SMTP_PASS=your_app_password

CLIENT_URL=http://localhost:5173
VITE_DEV_MODE=true
```

### 2. Backend Installation
```bash
npm install
cd server && node server.js
```

### 3. Frontend Installation
```bash
cd client
npm install
npm run dev
```

### 4. Seed Data
Populate the database with luxury skincare products:
```bash
node seed/seed.js
```

## ✨ Key Features
- **OTP Login:** Secure, passwordless entry.
- **AI Recommendations:** Similarity-based product discovery.
- **Admin Dashboard:** Real-time revenue analytics and product/order management.
- **Automated Invoices:** Professional PDF invoices generated on payment success.
- **Omni-channel Alerts:** Email and WhatsApp notifications for every completed ritual.

---
*Veda Aura: The bridge between ancient wisdom and modern radiance.*
