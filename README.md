# habitflow 🌿

A clean, minimal habit tracker with Firebase authentication and streak tracking.

**Live Demo:** [your-project.vercel.app](https://your-project.vercel.app)

---

## What it does

- Sign up / log in with email & password or Google
- Add daily habits and check them off each day
- Track your current streak per habit
- See your weekly progress at a glance
- Data is saved per user in the browser

---

## Tech Stack

| | |
|---|---|
| Frontend | HTML, CSS, Vanilla JavaScript |
| Auth | Firebase Authentication (Email/Password + Google OAuth) |
| Storage | Browser `localStorage` (per Firebase UID) |
| Fonts | Google Fonts — DM Serif Display + DM Sans |
| Hosting | Vercel + GitHub |

---

## Project Structure

```text
habitflow/
├── auth.html
├── dashboard.html
└── README.md