<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=180&section=header&text=Glamr%20%E2%80%94%20Beauty%20Connect%20AI&fontSize=38&fontColor=fff&animation=twinkling&fontAlignY=32&desc=AI-Powered%20Beauty%20Salon%20Marketplace%20%7C%20Bangalore&descAlignY=62&descSize=16" alt="Glamr Banner"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=1000&color=F472B6&center=true&vCenter=true&width=750&lines=AI-Powered+Beauty+Salon+Marketplace+%F0%9F%92%84;43+Premium+Salons+across+Bangalore+%F0%9F%8C%86;React+%2B+Firebase+%2B+MVC+Architecture+%F0%9F%9A%80;Built+for+SuperXgen+AI+Startup+Buildathon+2026+%F0%9F%8F%86" alt="Typing SVG"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React.js-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React"/>
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase"/>
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind"/>
  <img src="https://img.shields.io/badge/MVC_Architecture-F472B6?style=flat-square&logoColor=white" alt="MVC"/>
  <img src="https://img.shields.io/badge/Version-2.0-38BDF8?style=flat-square" alt="Version"/>
  <img src="https://img.shields.io/badge/Hackathon-SuperXgen_2026-BF91F3?style=flat-square" alt="Hackathon"/>
</p>

---

## 📌 Overview

**Glamr** is a full-stack, AI-powered beauty salon marketplace built for Bangalore — allowing users to discover premium salons, get AI-matched stylist recommendations, book appointments, and manage their beauty experience end-to-end.

Built in 48 hours for the **SuperXgen AI Startup Buildathon 2026** by a 3-member team using React.js, Firebase, and a clean MVC architecture.

---

## ✨ Features

| Category | Features |
|---|---|
| 🏠 **Home** | 4-slide auto-carousel hero slider with arrows, dots & smooth transitions |
| 💇 **Salon Discovery** | 43 premium salons across 12+ Bangalore areas with area filters & service chips |
| 🤖 **AI Stylist Finder** | AI-powered salon recommendations based on user preferences |
| 🔐 **Authentication** | Split-screen Login/Signup with glassmorphism UI & password visibility toggle |
| 📅 **Booking System** | Full appointment booking, confirmation & history management |
| 💳 **QR Payment Flow** | QR-based payment screen with booking confirmation |
| 📊 **Customer Dashboard** | Upcoming appointments, booking history & favourite salons |
| ⭐ **Reviews & Ratings** | Per-salon reviews and rating system |
| 📞 **Contact Page** | Contact form, FAQ section & full contact details |
| ⚡ **Performance** | Lazy-loaded routes via `React.lazy` + shimmer skeleton loaders |
| 📱 **Responsive UI** | Luxury-grade responsive design across all screen sizes |

---

## 🏗️ Architecture

This project follows a strict **MVC (Model-View-Controller)** pattern for clean separation of concerns and maintainability.

```
src/
├── models/                   # Pure data layer
│   ├── SalonModel.js
│   ├── BookingModel.js
│   ├── UserModel.js
│   └── ReviewModel.js
│
├── controllers/              # Business logic hooks
│   ├── useAuthController.js
│   ├── useSalonController.js
│   ├── useBookingController.js
│   └── useAIController.js
│
├── services/
│   ├── firebase/             # Firebase config, auth & salon services
│   │   ├── firebaseConfig.js
│   │   ├── authService.js
│   │   └── salonService.js
│   └── api/                  # AI service & mock salon data (43 salons)
│       ├── aiService.js
│       └── mockData.js
│
├── views/
│   ├── components/
│   │   ├── layout/           # Navbar (sticky/scroll-aware), Footer
│   │   ├── ui/               # SalonCard, HeroSlider
│   │   └── common/           # Spinner, Toast, PrivateRoute, AdminRoute
│   └── pages/                # All pages (lazy-loaded)
│
├── utils/                    # constants.js, helpers.js
├── styles/                   # global.css (design tokens)
└── App.jsx                   # Root router + Auth wiring
```

---

## 🛠️ Tech Stack

**Frontend**

![React](https://img.shields.io/badge/React.js-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![React Router](https://img.shields.io/badge/React_Router-CA4245?style=flat-square&logo=reactrouter&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)

**Backend & Database**

![Firebase](https://img.shields.io/badge/Firebase_Auth-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Firestore](https://img.shields.io/badge/Cloud_Firestore-FF6F00?style=flat-square&logo=firebase&logoColor=white)

**Architecture & Performance**

![MVC](https://img.shields.io/badge/MVC_Pattern-F472B6?style=flat-square)
![Lazy Loading](https://img.shields.io/badge/React.lazy-61DAFB?style=flat-square&logo=react&logoColor=black)
![Skeleton](https://img.shields.io/badge/Skeleton_Loaders-38BDF8?style=flat-square)

---

## 🚀 Getting Started

### Prerequisites
- Node.js v16+
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/21vicky/Beauty-Connect-AI.git

# Navigate into the project
cd Beauty-Connect-AI

# Install dependencies
npm install

# Start the development server
npm start
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

> ✅ Works out-of-the-box with **43 mock salons** — no Firebase API keys required to run locally.

---

## ⚙️ Configuration

### Firebase Setup

Edit `src/services/firebase/firebaseConfig.js` with your Firebase project credentials.

To toggle between **mock data** and **live Firestore data**, update the flag in:
```
src/services/firebase/salonService.js
```

### Environment Variables

Create a `.env` file in the project root:

```env
REACT_APP_FIREBASE_API_KEY=your_key
REACT_APP_FIREBASE_AUTH_DOMAIN=your_domain
REACT_APP_FIREBASE_PROJECT_ID=your_project_id
REACT_APP_FIREBASE_STORAGE_BUCKET=your_bucket
REACT_APP_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
REACT_APP_FIREBASE_APP_ID=your_app_id
REACT_APP_ANTHROPIC_API_KEY=your_anthropic_key
```

> ⚠️ Never commit your `.env` file — it is already added to `.gitignore`.

---

## 💳 Payment Flow

```
Booking Page → Payment Page (QR Code) → Booking Confirmation
```

- QR payment powered by `react-qr-code`
- Payment screen: `src/views/pages/PaymentPage.jsx`
- Confirmation: `src/views/pages/BookingConfirmPage.jsx`

---

## 💇 Salon Coverage

**43 premium salons across 12+ Bangalore areas**

| Brand | Count |
|---|---|
| Bodycraft | 8 |
| Lakme Salon | 6 |
| YLG Salon | 5 |
| Naturals | 4 |
| Enrich Salon | 4 |
| BBLUNT, JCB, Blown, Franck Provost, Jawed Habib | 2 each |
| Toni & Guy, Mirrors, Alchemic, BarberCo, Straight Salon, Studio 11, Green Trends | 1 each |

---

## 👥 Team

Built with 💜 for the **SuperXgen AI Startup Buildathon 2026**

| Name | Role | GitHub |
|---|---|---|
| Vignesh U | Full Stack & AI Integration | [@21vicky](https://github.com/21vicky) |
| Sri Thirumalai Vasan S | Frontend & UI/UX | [@Sri-Thirumalaivasan](https://github.com/Sri-Thirumalaivasan) |
| Ramesh Babu V | Frontend & Firebase | [@Ramesh118-hue](https://github.com/Ramesh118-hue) |

---

## 📄 License

This project was built for hackathon purposes. All rights reserved by the team.

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=120&section=footer&animation=twinkling" alt="Footer"/>
</p>

<p align="center">
  Made with 💄 for <strong>SuperXgen AI Startup Buildathon 2026</strong>
</p>
