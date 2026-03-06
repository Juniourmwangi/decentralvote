# 🇰🇪 DecentralVote — IEBC Blockchain Voting System

A blockchain-powered electronic voting platform built for the **Independent Electoral and Boundaries Commission (IEBC)** of Kenya. DecentralVote eliminates human interference in the voter approval process using automated cryptographic verification.

---

## 🚀 Features

- **Auto-Verified Registration** — No admin can approve or reject voters. The system validates National IDs automatically using a 5-step cryptographic process
- **Blockchain Ledger** — Every vote is recorded as an immutable block on SimChain v1
- **One Wallet, One Vote** — Each approved voter receives a unique blockchain wallet; duplicate voting is cryptographically impossible
- **Live Results** — Real-time vote tallies and percentage breakdowns per candidate
- **Zero Corruption** — Human gatekeeping is completely removed from the approval pipeline
- **Green-Themed UI** — High-contrast, accessible interface with clear readability

---

## 📁 Project Structure

```
decentralvote/
│
├── decentralvote.html     # Main application (single-file)
└── README.md              # This file
```

---

## 🛠️ How to Run

This is a **single HTML file** — no installation or server needed.

1. Download `decentralvote.html`
2. Open it in any modern browser (Chrome, Firefox, Edge)
3. That's it — it runs entirely in the browser

---

## 🗳️ How It Works

### Step 1 — Register
- Fill in your Full Name, National ID (8 digits), County, and Phone Number
- The system runs 5 automated checks:
  - ✅ ID format validation
  - ✅ IPRS database cross-reference
  - ✅ Duplicate detection
  - ✅ Cryptographic wallet generation
  - ✅ Voter record written to chain

### Step 2 — Connect Wallet
- Go to the **Vote tab**
- Click **Connect Wallet**
- Enter your National ID to authenticate

### Step 3 — Cast Your Vote
- Select your preferred candidate
- Your vote is mined as a new block on the chain
- The transaction hash is shown as your receipt

### Step 4 — View Results
- Visit the **Stats tab** for live results and registered voter list
- Visit the **Ledger tab** to see all blocks on the chain

---

## 🔐 Security Design

| Feature | Implementation |
|---|---|
| Voter approval | Fully automated — no human involvement |
| Duplicate prevention | National ID uniqueness enforced at registration |
| Vote integrity | Each vote hashed with previous block hash (chain linkage) |
| One vote per wallet | Wallet address checked against blockchain before voting |
| Wallet generation | Cryptographically random 40-character hex address |

---

## 🧱 Tech Stack

- **Frontend** — Pure HTML, CSS, JavaScript (no frameworks)
- **Fonts** — IBM Plex Mono + Outfit (Google Fonts)
- **Blockchain** — SimChain v1 (simulated in-browser blockchain)
- **Verification** — Client-side automated validation pipeline

---

## 📸 Screenshots

> Register tab with animated auto-verification → Vote tab with live candidate bars → Ledger showing mined blocks

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "feat: describe your change"`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

 Group members:

|Seth Nalwa — 23/08173 · BIT|
|Brian Nyamanga Otieno — 23/04444 · BIT|
|James Mwangi — 18/03989 · BBIT|
|Anne Wanjiku — 23/08081 · BBIT|
|Hongo Barnabas — 16/06034 · BBIT|
|Janice Cheruiyot — 22/06461 · BBIT|
