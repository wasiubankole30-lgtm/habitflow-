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

```
habitflow/
├── auth.html        # Login & sign up page
├── dashboard.html   # Main app (protected route)
└── README.md
```

---

## Running Locally

No build step needed. Just open `auth.html` in your browser:

```bash
# Option 1 — open directly
open auth.html

# Option 2 — serve with VS Code Live Server extension
# Right-click auth.html → Open with Live Server
```

> **Note:** Google Sign-In requires the page to be served over HTTP/HTTPS (not opened as a `file://` path). Use Live Server or deploy to Vercel.

---

## Deploying to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → **New Project** → Import your repo
3. No build configuration needed — Vercel will detect it as a static site
4. Set your production domain in Firebase:
   - Firebase Console → Authentication → Settings → **Authorized Domains**
   - Add your Vercel domain (e.g. `your-project.vercel.app`)

---

## Firebase Setup Note

The Firebase config in this repo is intentionally public — this is normal for Firebase web apps. Firebase security rules and authorized domains control who can actually use the project. If you fork this repo and want your own Firebase project:

1. Create a project at [firebase.google.com](https://firebase.google.com)
2. Enable **Authentication** → Email/Password and Google providers
3. Replace the `firebaseConfig` object in both `auth.html` and `dashboard.html` with your own config

---

## Known Limitations

- **Data is device-local** — habits are stored in `localStorage`, so they won't sync across different devices or browsers. A future version could use Firestore for cloud sync.
- **Stats & Settings tabs** — visible in the bottom nav but not yet implemented (planned for a future update).

---

## Planned Features

- [ ] Firestore sync (cross-device data)
- [ ] Stats page — habit completion charts and history
- [ ] Settings — edit or reorder habits
- [ ] Reminders / push notifications

---

## Screenshots

> Add screenshots here after deployment

---

## License

MIT
