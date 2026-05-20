# 🛒 AI-Powered Ecommerce Checkout Recovery System

**B.Tech Project | Machine Learning + Full Stack | Checkout Abandonment Recovery**

---

## 🔍 Overview

This repository contains a full-stack machine learning project designed to **reduce checkout abandonment** in ecommerce platforms through predictive analytics and intelligent recovery workflows.

The system monitors customer activity during checkout, predicts the likelihood of abandonment using a trained ML model, and activates recovery strategies such as discounts, shipping assistance, and AI-powered customer interaction.

> **Problem Addressed:** Customers adding products to the cart but leaving before completing payment — one of the most common and costly problems in ecommerce.

**Fictitious Store:** ShopSmart Pvt. Ltd.  
**Stack:** Python · FastAPI · Scikit-learn · HTML/CSS/JS  
**ML Model:** Random Forest Classifier  

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `backend/main.py` | ⚙️ FastAPI backend — prediction & recovery APIs |
| `ml/train_model.py` | 🤖 ML pipeline — model training & export |
| `ml/model.pkl` | 📦 Trained Random Forest model |
| `frontend/index.html` | 🖥️ Checkout interface with behavior tracking |
| `dashboard/analytics.html` | 📊 Merchant analytics dashboard |
| `README.md` | 📖 This file |

---

## 🔄 Recovery Workflow

```
Customer Enters Checkout
        ↓
Behavior Tracking Starts  ←— Idle Time | Tab Switch | Payment Interaction
        ↓
ML Model Predicts Risk  ←— Cart Value | Exit Intent | Checkout Duration
        ↓
High Abandonment Risk?
        ↓
Recovery Workflow Activates  ←— Discount | Shipping Help | AI Chatbot
        ↓
✅ Checkout Completed
```

---

## ✨ Key Features

- 🔮 **Real-time abandonment prediction** using a trained Random Forest model
- 🧾 **Dynamic checkout interface** with editable pricing and coupon handling
- 🤖 **AI-powered recovery assistant** with smart intervention suggestions
- ⚡ **FastAPI backend** for prediction, chatbot support, and recovery logic
- 📊 **Merchant analytics dashboard** with recovery metrics and risk monitoring

---

## 🧠 ML Feature Set

| Feature | Description |
|---------|-------------|
| `cart_value` | Total value of items in cart |
| `idle_time` | Seconds customer has been inactive |
| `payment_failures` | Number of failed payment attempts |
| `exit_intent` | Mouse movement toward browser close/tab |
| `checkout_duration` | Total time spent on checkout page |

---

## 💻 How to Run Locally

### Option A — Run Frontend Only

1. Clone the repository:

```bash
git clone https://github.com/rishavsingh1k/AI_checker
cd AI_checker
```

2. Open the frontend code in your browser:

```
kas.html
```

### Option B — Run Full Stack

1. Install backend dependencies:

```bash
pip install fastapi uvicorn scikit-learn pandas
```

2. Start the FastAPI server:

```bash
uvicorn backend.main:app --reload
```

3. Open `frontend/index.html` in your browser.

---

## 🏗️ System Architecture

```
[ Frontend — HTML/CSS/JS ]
        ↓  (REST API calls)
[ FastAPI Backend ]
        ↓
[ ML Model — RandomForestClassifier ]
        ↓
[ Recovery Engine — Discount / Shipping / Chatbot ]
```

The architecture intentionally separates frontend interaction handling from backend intelligence — improving scalability and reflecting how real-world ecommerce platforms are structured.

DEMO LINK (Project narration with screen recording)
-------------https://drive.google.com/file/d/1nWrwWWyrEEhUvK1AFgUMx1tlzFOPEHIE/view?usp=sharing--------------------------
