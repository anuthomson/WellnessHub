# 🌿 WellnessHub

**A full-stack personal wellness platform where users track their health, read wellness articles and get support from providers, all in one dashboard.**

![React](https://img.shields.io/badge/React%2019-61DAFB?logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express%205-000000?logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white)
![JWT](https://img.shields.io/badge/Auth-JWT-orange)

---

## ✨ Features

**Health trackers**
- 💧 Water intake · ⚖️ Weight · 😴 Sleep · ❤️ Heart rate
- 🚶 Walking and 🏃 exercise / activities
- 😊 Daily mood check-in
- 🥗 Meal plans and recipes

**Content & community**
- 📰 Wellness articles (written in Markdown) with likes

**Accounts & roles**
- Register and log in with **bcrypt-hashed passwords** and **JWT** authentication
- Separate dashboards for **users**, **providers** and **admins**
- Admin tools for managing accounts and articles

## 🏗️ Architecture

```
wellnesshub-frontend/  (React 19 + React Router)   ──HTTP/JSON──▶   Express 5 REST API   ──▶   MongoDB (Mongoose)
        port 3001                                                    port 3000
```

**Back end:** `routes/` → `controllers/` → `models/`, with `auth.middleware.js` protecting private endpoints.

## 🔌 API

`/api/accounts` · `/api/articles` · `/api/likes` · `/api/water` · `/api/weight` · `/api/sleep` · `/api/heartrate` · `/api/walking` · `/api/activities` · `/api/mood` · `/api/mealplans`

## 🚀 Run it

**1. Back end**
```bash
cd WellnessHub
npm install
# create a .env file with your MongoDB connection string and JWT_SECRET
npm run dev          # http://localhost:3000
```

**2. Front end**
```bash
cd WellnessHub/wellnesshub-frontend
npm install
npm start            # http://localhost:3001
```

## 📄 Project documents

The [`Design/`](Design), [`System proposal/`](System%20proposal) and [`Final report/`](Final%20report) folders hold the system proposal, scope document, system design, class diagram and final report.

---

👥 Team project for **CP3540 (Applied ASD Project)**, College of the North Atlantic.
Original repository: [auditorydamage/CP3540_Team_1](https://github.com/auditorydamage/CP3540_Team_1)
👩‍💻 Team member: **[Anumol Thomas](https://github.com/anuthomson)**
