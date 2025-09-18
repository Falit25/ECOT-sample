# 🌱 EcoTrack: Smart Sustainability Score Card

[![Node.js](https://img.shields.io/badge/Node.js-18+-brightgreen.svg)](https://nodejs.org/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Compatible-blue.svg)](https://www.postgresql.org/)
[![Security](https://img.shields.io/badge/Security-Enhanced-green.svg)](https://github.com/yourusername/ecotrack)

A full-stack sustainability platform that helps users track and reduce their carbon footprint through gamification and rewards.

## 🚀 Quick Start

```bash
# Install and run
npm install
npm start

# Open browser
http://localhost:3000
```

## ✨ Features

- **🧮 Carbon Calculator** - 4-section assessment (4-16 tons CO₂/year)
- **🎮 Weekly Games** - Plant Tracker, Recycle Quest, Energy Saver (+5 pts each)
- **🏆 Rewards Store** - Digital badges (200pts), Stickers (500pts), Products (1000pts)
- **📊 3D Visualizations** - Interactive charts powered by Plotly.js
- **🔧 Admin Panel** - User management, reward processing, analytics
- **🔐 Security** - JWT auth, rate limiting, input validation

## 🛠️ Tech Stack

**Backend:** Node.js, Express, PostgreSQL, JWT, bcrypt  
**Frontend:** HTML5, CSS3, Vanilla JS, Plotly.js  
**Security:** Rate limiting, SSL validation, safe DOM manipulation

## 📁 Structure

```
SSH/
├── complete-server.js    # Main server
├── index.html           # Landing page
├── login.html           # Authentication
├── dashboard.html       # User dashboard
├── calculator.html      # Carbon calculator
├── rewards.html         # Rewards store
├── admin.html          # Admin panel
├── css/style.css       # Styles
└── js/quiz.js          # Quiz logic
```

## ⚙️ Setup

**Environment (.env):**
```env
DATABASE_URL=postgresql://user:pass@host:port/db
JWT_SECRET=your-secret-key
ADMIN_PASSWORD=admin123
PORT=3000
```

**Database:** Auto-creates tables on first run

## 🎯 Usage

1. **Register/Login** → **Take Calculator** (+10 pts) → **Play Games** (+5 pts each)
2. **Admin:** `/admin.html` (password: admin123) → Manage users & rewards

## 🔒 Security & Accuracy

**Security Fixes Applied:**
- ✅ Code injection prevention (safe DOM methods)
- ✅ SSL certificate validation
- ✅ Input validation middleware
- ✅ Rate limiting (5 attempts/5min)
- ✅ Path traversal protection
- ✅ Timing-safe password comparison

**Carbon Footprint Accuracy:**
- 🟢 **Low Impact (4-7 tons)**: Eco-conscious lifestyle
- 🟡 **Medium Impact (7-12 tons)**: Near global average
- 🔴 **High Impact (12-16+ tons)**: High consumption

**Formula:** `4 + (score-40)/(200-40) * (16-4)` tons CO₂/year

## 🐛 Troubleshooting

- **Port in use**: Change PORT in `.env`
- **Dependencies**: Run `npm install`
- **Admin login**: Default password `admin123`
- **Database**: Auto-creates tables on startup

---

**🌐 Server:** http://localhost:3000 | **🔐 Admin:** /admin.html (admin123)

*Built with 💚 for a sustainable future*