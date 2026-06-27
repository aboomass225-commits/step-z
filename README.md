# 👟 STEP_Z — Full Stack E-Commerce

## 🚀 HOW TO RUN (Windows)

### Step 1: Install Node.js
- Go to: https://nodejs.org
- Download & install LTS version

### Step 2: Install MongoDB
- Go to: https://www.mongodb.com/try/download/community
- Download & install MongoDB Community
- OR use MongoDB Atlas (free cloud): https://cloud.mongodb.com

### Step 3: Setup Project
Open Command Prompt (CMD) in STEP_Z folder:
```
cd C:\path\to\STEP_Z
npm install
```

### Step 4: Configure .env
Open `.env` file and update:
```
MONGO_URI=mongodb://localhost:27017/stepz_db
RAZORPAY_KEY_ID=rzp_test_YOUR_KEY
RAZORPAY_KEY_SECRET=YOUR_SECRET
```

### Step 5: Start Server
```
npm run dev
```

### Step 6: Open Website
Go to: http://localhost:5000

### Step 7: Seed Database (First time)
Open browser → go to: http://localhost:5000
Admin login: admin@stepz.com / Admin@123

---

## ✅ FEATURES

### Customer:
- Browse shoes, slippers, sandals, sports, kids
- Search products
- Add to cart
- Wishlist
- Checkout (Razorpay + COD)
- Order tracking
- User profile

### Admin Panel (/admin):
- Dashboard with stats
- Add products with REAL PHOTOS
- Edit product (name, price, stock, images)
- Delete products
- View & update all orders
- Manage users

---

## 📁 PROJECT STRUCTURE
```
STEP_Z/
├── backend/
│   ├── server.js          ← Main server
│   ├── config/db.js       ← MongoDB
│   ├── models/
│   │   ├── User.js
│   │   ├── Product.js
│   │   └── Order.js
│   ├── routes/
│   │   ├── auth.js        ← Login/Register
│   │   ├── products.js    ← Products + Image Upload
│   │   ├── orders.js      ← Orders + Tracking
│   │   └── payment.js     ← Razorpay
│   ├── middleware/auth.js
│   └── uploads/           ← Product images saved here
├── frontend/
│   └── index.html         ← Full website
├── .env
└── package.json
```

## 🔑 RAZORPAY SETUP
1. Go to: https://dashboard.razorpay.com
2. Register free account
3. Go to Settings → API Keys
4. Copy Key ID & Secret to .env

Made with ❤️ — STEP_Z 2025
