# Arbitrum.Labs - Cryptographic Mining Simulator

An interactive, client-side **Proof-of-Work (PoW) Mining Simulator** designed to visually demonstrate the core mechanics of blockchain technology, cryptographic hashing, and chain immutability.

---

## 🚀 Features

* **Real-Time SHA-256 Hashing:** Utilizes the browser's native Web Crypto API to calculate cryptographic hashes instantly as you type.
* **Proof-of-Work Simulation:** Includes a local mining loop that increments a block's nonce until it matches the network difficulty target (a `00` prefix).
* **The Domino Effect:** Demonstrates blockchain immutability in real time. Changing data in the Genesis Block automatically breaks the cryptographic link, invalidating all subsequent blocks.
* **Modern UI/UX:** Styled with a responsive, dark-mode dashboard layout using Tailwind CSS, featuring active state transitions (Emerald for valid blocks, Rose for invalid blocks).

---

## 🛠️ Tech Stack

* **Frontend Framework:** HTML5, JavaScript (ES6+)
* **Styling Engine:** [Tailwind CSS v4](https://tailwindcss.com/) (via runtime browser script)
* **Cryptography Engine:** Native Web Crypto API (`crypto.subtle.digest`)

---

## 📖 How It Works

1. **Data Payload:** Input transaction text or arbitrary records into any block's data field.
2. **The Nonce:** Manually tweak the nonce value, or let the machine do it for you.
3. **Mining:** Click the **Mine Block** button to simulate computational energy consumption. The engine cycles through nonces until the hash satisfies the target difficulty criteria.
4. **Validation:** Watch Block 2 grab the output hash of Block 1 as its `Previous Hash`. Tampering with old data breaks the visual chain link instantly.

---

## 📂 Installation & Deployment

Since this project runs entirely on the client side without external backend dependencies, deployment is trivial:

1. Clone or download this repository.
2. Open the `simulator.html` file directly in any modern web browser.

