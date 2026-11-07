# 🌴 The Oasis — People & Entertainment Social Lounge

**The Oasis** is a people-first, entertainment-oriented social lounge designed to escape the algorithmic noise. Built with **HTML5, Tailwind CSS, Canvas Confetti, and Google Firebase (Auth + Cloud Firestore)**.

---

## 🌟 What Makes The Oasis Different?

- **🌴 People & Good Vibes Only:**
  - Designed around cinema, music, gaming, weekend plans, and wholesome memes.
  - Interactive **Cheers & Confetti** celebrations on likes and connections.
  - Category filters: `🎵 Music & Drops`, `🍿 Cinema & Shows`, `🎮 Gaming Den`, and `🎭 Memes & Laughs`.
- **📻 The Oasis Lounge Radio:**
  - Built-in lounge vibe player card with one-click cheers and community tunes.
- **🔐 Google Sign-In with Firebase Authentication:**
  - Sign in with your real Google account via one-click popup.
  - Automatically loads your Google profile photo, display name, and handle.
- **⚡ Real-Time Cloud Firestore Sync:**
  - Share vibes, memes, and photos that broadcast across all active visitors live without refreshing.
- **🎮 Instant Demo Mode:**
  - Works immediately out of the box in Chrome using simulated Google login and local storage until you connect your Firebase keys.

---

## 🚀 1. Run it Locally in Chrome

### Quick Direct Open:
Press `Win + R`, paste this command, and press Enter:
```cmd
chrome "C:\Users\Tyler\.gemini\antigravity\scratch\x-clone-firebase\index.html"
```

### Or With a Local Server (Recommended for Google OAuth):
```powershell
cd C:\Users\Tyler\.gemini\antigravity\scratch\x-clone-firebase
python -m http.server 3000
```
Then visit `http://localhost:3000` in Chrome.

---

## 🌐 2. Live GitHub Pages Deployment

Your repository is connected to:
🔗 **https://github.com/tylerrnmn/pulse-social**

To update your live site:
```powershell
cd C:\Users\Tyler\.gemini\antigravity\scratch\x-clone-firebase
git add .
git commit -m "feat: rebrand to The Oasis social lounge"
git push -u origin main
```

Your live site link:
🌴 **https://tylerrnmn.github.io/pulse-social/**
*(Give GitHub Pages 1–2 minutes after pushing to complete the build!)*
