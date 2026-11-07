# 🐦 Pulse — X (Twitter) Clone with Google Firebase

A modern, responsive microblogging web application designed to look and feel like **X (Twitter)** with **Google Sign-In** and **Cloud Firestore** for real-time posts.

---

## ✨ Features

- **Iconic 3-Column X Layout:**
  - Left navigation bar (Home, Explore, Notifications, Bookmarks, Profile).
  - Central interactive compose box and live real-time timeline feed.
  - Right sidebar with Search, Trending topics, and "Who to Follow" recommendations.
- **Google Sign-In with Firebase Authentication:**
  - Authenticate with your real Google account via Firebase OAuth popup.
  - Automatically loads your Google profile picture, display name, and handle.
- **Real-Time Posts with Cloud Firestore:**
  - Posts publish instantly and update the feed in real-time across all connected browser tabs.
- **Interactive Post Features:**
  - Character counter (280 characters limit warning).
  - Like button with animation and counter.
  - Repost / Retweet button with counter.
  - Image / GIF attachment preview.
  - Follow / Unfollow toggle buttons.
- **Zero-Friction "Instant Demo Mode":**
  - Runs out of the box with zero setup in Chrome using simulated Google login and local storage until you configure your Firebase credentials!

---

## 🚀 1. Run it Locally in Chrome Right Now

Because Google OAuth security requires an HTTP origin (rather than `file:///`), you can run a quick local web server or open the file directly:

### Option A: Local Server (Recommended for Google OAuth popup)
Open PowerShell in this directory:
```powershell
cd C:\Users\Tyler\.gemini\antigravity\scratch\x-clone-firebase
npx serve .
# or if you have Python:
python -m http.server 3000
```
Then open Chrome to `http://localhost:3000`.

### Option B: Direct File Open (For Instant Demo Mode)
Press `Win + R`, paste this command and press Enter:
```cmd
chrome "C:\Users\Tyler\.gemini\antigravity\scratch\x-clone-firebase\index.html"
```

---

## 🔑 2. How to Set Up Your Free Google Firebase Backend

Connecting your real Google Firebase backend takes about 2 minutes:

1. **Create a Firebase Project:**
   - Go to the [Firebase Console](https://console.firebase.google.com/) and click **Add project**.
   - Name it (e.g. `pulse-social`) and complete the creation wizard.

2. **Enable Google Authentication:**
   - In the left sidebar, click **Build &rarr; Authentication**.
   - Click **Get Started**, then select **Google** from the Sign-in providers.
   - Toggle **Enable**, select your support email, and click **Save**.

3. **Enable Cloud Firestore Database:**
   - In the left sidebar, click **Build &rarr; Firestore Database**.
   - Click **Create database**, select a region close to you, and start in **Test mode** (allows read/writes during development).
   - Click **Create**.

4. **Register a Web App to Get Keys:**
   - Click the **Gear icon (Project settings)** at the top left.
   - Scroll down to "Your apps" and click the **Web icon (`</>`)**.
   - Give it a nickname (e.g. `Pulse Web`) and click **Register app**.
   - You will see a `firebaseConfig` block with `apiKey`, `authDomain`, `projectId`, etc.

5. **Connect It in Pulse:**
   - Open Pulse in Chrome.
   - Click **"Firebase Setup"** in the left sidebar or the **"Configure Firebase Keys"** card on the right.
   - Paste your configuration keys and click **Save & Connect**!

---

## 🌐 3. Publish to GitHub Pages

1. Create a new repository on [github.com/new](https://github.com/new) called `pulse-social` (Public).
2. Open PowerShell in this folder:
   ```powershell
   cd C:\Users\Tyler\.gemini\antigravity\scratch\x-clone-firebase
   git init
   git add .
   git commit -m "feat: initial x clone with firebase"
   git branch -M main
   git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/pulse-social.git
   git push -u origin main
   ```
3. In your repo on GitHub, go to **Settings &rarr; Pages**:
   - Set **Source** to `Deploy from a branch`.
   - Set **Branch** to `main` and folder to `/ (root)`.
   - Click **Save**.
4. In the **Firebase Console &rarr; Authentication &rarr; Settings &rarr; Authorized Domains**, add:
   `<YOUR_GITHUB_USERNAME>.github.io`
   *(This authorizes Google Sign-In to run from your live GitHub Pages URL!)*

Your live social app is now ready to share at:
```
https://<YOUR_GITHUB_USERNAME>.github.io/pulse-social/
```
