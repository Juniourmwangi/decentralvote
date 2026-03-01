# 🇰🇪 DecentralVote — Blockchain-Powered Voting System

> A decentralized, tamper-proof voting application inspired by Kenya's **Independent Electoral and Boundaries Commission (IEBC)**, built on blockchain principles.

---

## 📌 Project Overview

DecentralVote is a frontend simulation of a blockchain-based voting system that demonstrates how decentralized technology can solve real problems in Kenya's electoral process — including voter fraud, double voting, lack of transparency, and result manipulation.

Every vote cast in this system is stored as an **immutable block** on a simulated blockchain, linked to the previous block via a cryptographic hash — meaning no vote can be altered or deleted once recorded.

---

## 🚨 The Problem It Solves

Kenya's traditional voting systems face serious challenges:

- **Voter fraud** — people voting multiple times
- **Fake results** — tallies manipulated after voting
- **No transparency** — voters cannot verify their vote was counted
- **Corruption** — officials can alter records

DecentralVote addresses all of these using blockchain technology.

---

## ✅ Features

### 📝 Voter Registration
- Voters submit their **Full Name**, **National ID**, **County**, and **Phone Number**
- Registration is stored as a pending application
- Duplicate National IDs are rejected automatically

### 🔐 Admin Panel
- Secured with a password
- Admin can **Approve** or **Reject** voter registrations
- Each approved voter is automatically assigned a unique **blockchain wallet address**
- Admin can track who has voted and who hasn't in real time

### 🗳 Voting
- Voters connect using their **National ID**
- Only **approved** voters can access the ballot
- Each wallet can cast **exactly one vote** — enforced by the blockchain
- Pending and rejected voters are blocked with a clear message

### ⛓ Live Blockchain Ledger
- Every vote creates a new **block** with:
  - Block number
  - Voter wallet address
  - Cryptographic hash (linked to previous block)
  - Candidate voted for
  - Timestamp
- The ledger is **publicly visible** — anyone can audit the results

---

## 🔗 How Blockchain Works in This App

```
[Genesis Block #0]
       ↓
[Block #1] — Voter: 0x3f2a...8c1d | Candidate: Alice Mwangi | Hash: 0xa3f91b2c...
       ↓
[Block #2] — Voter: 0x7b4e...2f9a | Candidate: Carol Njeri  | Hash: 0xd72e4a1f...
       ↓
[Block #3] — ...
```

Each block contains the **hash of the previous block**, making it impossible to alter any vote without breaking the entire chain.

---

## 🖥 How to Use the App

### As a Voter
1. Go to the **Register tab**
2. Fill in your Name, National ID, County, and Phone
3. Submit and wait for admin approval
4. Once approved, go to the **Vote tab**
5. Click **Connect Wallet** and enter your National ID
6. Select your candidate and click **Cast Vote**
7. Check the **Ledger tab** to verify your vote is on the chain

### As an Admin
1. Go to the **Admin tab**
2. Enter password: `admin123`
3. Review pending registrations
4. Click **✓ Approve** or **✕ Reject** for each voter
5. Monitor the approved voters list to see who has voted

---

## 🛠 Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Structure |
| CSS3 | Styling (IEBC green theme) |
| Vanilla JavaScript | Blockchain simulation logic |
| Google Fonts (Syne + Space Mono) | Typography |
| GitHub Pages | Hosting |

> **Note:** This is a frontend simulation. A production version would use **Ethereum**, **Solidity smart contracts**, and **MetaMask** for real wallet authentication.

---

## 📁 Project Structure

```
decentralvote/
│
├── index.html        ← Main application (all-in-one file)
└── README.md         ← This file

## 📚 Concepts Demonstrated

| Blockchain Concept | How It's Shown |
|---|---|
| Immutability | Votes cannot be edited once cast |
| Chain linking | Each block stores the previous block's hash |
| Wallet identity | One National ID = one wallet = one vote |
| Transparency | Public ledger visible to everyone |
| Decentralization | No single entity controls the results |
| Smart contract logic | Admin approval before voting is unlocked |

---

## 🎓 Academic Context

This project was built as part of a **Blockchain & Decentralized Applications** course. The group identified **electoral fraud and lack of voting transparency** as a key problem in Kenya and proposed a blockchain-based solution modeled after the IEBC's mandate.

---

## 👥 Group Members

| Name | 
|---|---|
| [Seth Nalwa 23/08173  BIT]
| [Brian Nyamanga Otieno 23/04444  BIT]
| [James Mwangi 18/03989 BBIT] 
| [Anne wanjiku 23/08081 BBIT] | 
