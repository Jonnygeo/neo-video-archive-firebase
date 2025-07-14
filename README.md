# Neo Video Archive (Firebase Edition)

🧠 Built by Jonathan for the NeoLegacy AI Platform — where memory meets mission.

This version replaces Mux with Firebase Hosting and Storage for those who want to upload, store, and play back legacy video messages **without requiring a paid Mux account**.

---

## 📦 Features

- 🔐 Encrypted Video Upload via Firebase
- 🎥 Self-hosted playback with simple HTML5 `<video>` element
- 🧠 Metadata tagging for delivery intent (e.g., child ID, future date)
- 🌐 Firebase Hosting + Storage (free-tier eligible)
- 📁 JSON-based metadata structure (`video_metadata.json`)

---

## 🧠 How It Works

1. User uploads a video memory (via browser form)
2. Metadata is saved in `video_metadata.json`
3. Video is stored in Firebase Storage
4. Playback is controlled manually or via script logic (future delivery)

---

## 🚀 Quick Start (Firebase Setup)

> Skip Mux — just use Firebase to host and store.

```bash
npm install -g firebase-tools
firebase login
firebase init
# Choose: Hosting + Storage
# Public dir: public
# Single-page app: No
firebase deploy
