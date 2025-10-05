# EcoPledge Tracker — README

## 🌱 Overview
**EcoPledge Tracker** is a lightweight web app built for the **Hack 4 Humanity** hackathon. It simulates a blockchain ledger to record sustainability pledges transparently and demonstrate how blockchain can increase trust and accountability in environmental actions.

No setup required — open the HTML file in your browser, make pledges, and see how each pledge becomes a new block linked with SHA‑256 hashes. Any tampering breaks the chain until repaired, visually showing how blockchain integrity works.

---

## 💡 Theme Fit
This project aligns with the 2025 Hack 4 Humanity theme: **“Use blockchain to increase transparency, accessibility, or trust in sustainability.”**

EcoPledge Tracker uses a *simulated blockchain* to ensure each sustainability pledge is publicly verifiable and tamper‑resistant, encouraging accountability and transparency among communities.

---

## ⚙️ Features
- **Add pledges** — Record your name, category, and sustainability action.
- **Tamper detection** — Edit a past block and watch the chain become invalid.
- **Repair chain** — Re‑hash from a tampered block to restore validity.
- **Export/Import JSON** — Save or reload your blockchain state.
- **Local storage** — All data persists in the browser.

---

## 🧩 How It Works
Each block stores:
```js
{
  index: Number,
  timestamp: Date.now(),
  data: { name, pledge, category },
  previousHash: String,
  hash: String
}
```
The app computes each block’s hash using the browser’s built‑in **SHA‑256** algorithm. If any block’s data changes, its hash no longer matches and all subsequent links break — proving immutability.

---

## 🧪 How to Run
1. Download or clone this repo.
2. Open `index.html` in any browser.
3. Add a pledge and watch it appear in the blockchain table.
4. Try **Tamper → Repair** to test validation.
5. Use **Export JSON** to save your chain.

---

## 🎥 Demo Video Script (2–4 Minutes)
**Scene 1 – Intro (20s)**  
“Hi, I’m [Your Name], and this is *EcoPledge Tracker* — my project for Hack 4 Humanity 2025. It shows how blockchain can make sustainability pledges transparent and trustworthy.”

**Scene 2 – Add Pledge (40s)**  
“Here I add a pledge: ‘I’ll use public transport 3x a week.’ Each pledge becomes a new block with a SHA‑256 hash linked to the previous one. The chain stays valid.”

**Scene 3 – Tamper Test (40s)**  
“Now I’ll simulate tampering. I edit a past pledge — notice how the chain turns invalid. The hashes no longer match.”

**Scene 4 – Repair (40s)**  
“Clicking ‘Repair from here’ re‑hashes all blocks after the tampered one, restoring integrity — just like a blockchain.”

**Scene 5 – Wrap Up (30s)**  
“In a few minutes, EcoPledge Tracker proves how decentralized transparency can promote accountability in sustainability actions.”

---

## ✨ Future Enhancements
- Integrate real blockchain testnet (e.g., Polygon or Solana devnet)
- Add wallet support and signature verification
- Enable community leaderboards for collective pledges

---

## 🧾 License
MIT License — free to use and adapt for educational or non‑commercial hackathon projects.

---

**Built for Hack 4 Humanity 2025 — by [Your Name]**
