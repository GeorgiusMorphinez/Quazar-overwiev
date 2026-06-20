# Quazar – Digital Game Distribution Platform

**Quazar** is a full-featured online service for selling digital game products: games, applications, subscriptions, and accounts. It includes a web catalog, shopping cart, user library, admin panel, and a cross-platform launcher for Windows and Android.

This repository serves as a **navigation hub** for the entire project. It contains links to all components, documentation, and presentation materials.

---

## 🚀 Project Overview

- **Problem solved:** Lack of a unified platform in Russia and CIS for digital game distribution, leading to money outflow and technological dependence.
- **Goal:** Build a functional prototype with catalog, cart, library, admin panel, and launcher, supporting different product types and delivery mechanisms.
- **Result:** A fully working service, tested and documented, with a cross-platform launcher.

---

## 📦 Repository Components

| Component | Technology Stack | Repository |
|-----------|------------------|------------|
| **Backend** | Node.js, Express, Sequelize, PostgreSQL (Supabase), JWT, bcrypt, nodemailer, exceljs | [Quazar-server](https://github.com/GeorgiusMorphinez/Quazar-server) |
| **Frontend (Web)** | React, MobX, React Router, React-Bootstrap, Axios | [Quazar-client](https://github.com/GeorgiusMorphinez/Quazar-client) |
| **Launcher** | Flutter (Dart), WebView (Windows/Android), Inno Setup (installer) | [Quazar-launcher](https://github.com/GeorgiusMorphinez/Quazar-launcher) |

---

## 🧰 Key Technologies

- **Backend:** Node.js, Express, Sequelize, PostgreSQL (Supabase), JWT, bcrypt, nodemailer, exceljs, @supabase/supabase-js
- **Frontend:** React, MobX, React Router, React-Bootstrap, Axios, qrcode.react
- **Launcher:** Flutter, Dart, webview_flutter, webview_windows, Inno Setup
- **DevOps:** Railway (hosting), Supabase (database & storage), GitHub (version control)

---

## ✨ Main Features

- **Four product types:** Games, Applications, Subscriptions, Accounts
- **User authentication:** Registration, login, JWT-based sessions, password recovery (demo mode)
- **Catalog:** Filtering by type, tag, publisher; pagination
- **Shopping cart:** One-item limit per product, demo payment simulation
- **Orders & delivery:** Transactional order creation; automatic library entry for games/apps; subscription activation/renewal; account credentials delivery
- **Library:** Only accessible inside the launcher; shows purchased games/apps with active subscriptions and bought accounts
- **Admin panel:** Product, tag, publisher management; Excel report generation (visits, sales, popular tags, inventory)
- **Launcher:** Cross-platform (Windows/Android) with WebView; native back button support; custom User-Agent detection for library access

---

## 🛠️ How to Run Locally

### Backend
```bash
cd Quazar-server
npm install
cp .env.example .env   # fill in your database credentials
npm run dev
```
---

### Frontend
```bash
cd Quazar-client
npm install
npm start
```
---

### Launcher (Flutter)
```bash
cd Quazar-launcher
flutter pub get
flutter run -d windows   # or android
Note: The live demo hosted on Railway may be paused due to free-tier sleeping policy. The code is fully functional and can be run locally.
```
---

## 🧪 Testing
Extensive testing was performed:

Manual UI testing with both USER and ADMIN roles

API testing using Postman

Integration testing for checkout, subscription renewal, account delivery

All critical bugs (e.g., account ownership visibility) have been fixed

## 🏆 Diploma Project
This project was developed as a graduation thesis and defended with the highest grade ("Excellent") at the Novocherkassk Polytechnic College.

## 📫 Contact
GitHub: GeorgiusMorphinez

Email: alex09090909app.p@gmail.com
