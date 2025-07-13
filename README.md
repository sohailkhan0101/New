# New

# 🛒 Mood-Aware Shopping Concierge

> An AI-powered e-commerce prototype that senses user mood in real-time and adapts the shopping experience to reduce stress and decision fatigue. Built for mental well-being.

## 🎯 Problem
Many online shoppers—especially those with anxiety or decision paralysis—feel overwhelmed while browsing. This leads to cart abandonment, impulse buying, and stress. Current platforms rarely address mental well-being.


## 💡 Solution
This project leverages **real-time emotion detection** using webcam input and adaptive product recommendations to:

- Reduce choice overload during stressful moments
- Highlight “good enough” options to avoid overthinking
- Trigger mindful checkout tools during impulsive states
- Enforce a snooze/cooldown when needed

---

## 🌟 Features

| Core Capability          | Description                                               |
|--------------------------|-----------------------------------------------------------|
| 😃 Emotion Sensing        | Uses webcam + ML to detect stress, impulsivity, calmness |
| 🎯 Adaptive UI            | Limits or expands product options based on user mood     |
| 🛍️ Smart Recommendations | Top 3 picks for stressed users, full grid for calm users |
| 🧘 Mindful Checkout       | Prompts for impulse control, cooldown timers             |
| 📊 Real-Time Dashboard    | Emotion trend visualized using line chart                |
| 🔒 Auth + JWT             | Secure login/register system with form validation        |
| 🌐 Responsive UI          | Mobile-first, Tailwind CSS + accessible (WCAG) design     |

---

## 🛠 Tech Stack

- **Frontend**: React, TailwindCSS, Recharts, FaceAPI.js
- **Backend**: Python, FastAPI, SQLAlchemy, SQLite/PostgreSQL
- **ML/Emotion**: face-api.js (on-device facial expression detection)
- **APIs**: OpenAI (optional), Affectiva (future-ready)

---

## 🚀 Setup Instructions

### 🖥️ Backend
```bash
cd backend
pip install -r requirements.txt  # or manually: fastapi uvicorn sqlalchemy bcrypt python-jose
python productSeeder.py  # seed demo product data
uvicorn main:app --reload
```

### 💻 Frontend
```bash
cd frontend
npm install
npm start
```

### 📷 Models for FaceAPI.js
Place the following in `public/models/`:
- `tiny_face_detector_model`
- `face_expression_model`

Download from: https://github.com/justadudewhohacks/face-api.js-models

---

## 🧪 Demo Flow (Judges' MVP)
1. Login or Register
2. Webcam detects stress → UI adapts
3. Products shrink to top 3 suggestions
4. Try impulse click → mindful prompt activates
5. Dashboard shows emotion trends in real-time

---

## 📦 Sample Users
- Email: `test@example.com`
- Password: `password123`

---

## 🔐 Privacy & Ethics
- All emotion detection is processed **client-side**
- No biometric data is stored or transmitted
- GDPR-friendly architecture (optional opt-out ready)

---

## 📈 Future Enhancements
- Browser extension integration for any e-comm site
- Wearable heart-rate sensor sync (via Fitbit/Apple APIs)
- RAG-based recommendations using purchase context

---

## 💡 Authors & Credits
- 👨‍💻 Full-stack Engineering: [Your Name]
- 🎨 UI/UX & Accessibility: [Your Name or Team Member]
- 🧠 ML Integration: [Your Name or Team Member]

---

## 📄 License
MIT — Free to use for any ethical commercial or academic purpose.

---

### 🙌 Built with empathy at [Hackathon Name] 💙
