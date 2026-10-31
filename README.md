# Xplushop.luxfy — xplushop.xyz
> Gaming top-up storefront + secure Node.js + Stripe Checkout backend

![Node](https://img.shields.io/badge/Node.js-20+-339933?style=flat-square&logo=node.js&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-Checkout-635bff?style=flat-square&logo=stripe&logoColor=white)
![Express](https://img.shields.io/badge/Express-4.21-black?style=flat-square&logo=express)
![License](https://img.shields.io/badge/License-MIT-a78bfa?style=flat-square)

Public starter repo for **Xplushop** - Malaysia gaming top-up for 【entity-PUBG¦canonical_name=PUBG】 UC, MLBB Diamonds, 【entity-Free Fire¦canonical_name=Free Fire】 Diamonds.

**Live Domain:** xplushop.xyz  
**Style:** Dark Gaming / Purple Neon / Glassmorphism

---

### ✨ Features

- **Storefront:** Your supplied `index.html` preserved as homepage - dark gaming UI
- **Secure Checkout:** Stripe Checkout Sessions - prices validated server-side
- **Server:** Node.js 20 + Express + Helmet + Rate Limit
- **Webhooks:** Signed Stripe webhook verification (`/api/webhook`)
- **Catalog:** `src/catalog.js` - MYR sen pricing (590 = RM 5.90), never trust browser
- **CI:** GitHub Actions Node.js 20 test + check
- **Docs:** Architecture, Stripe setup, Deployment, Project backlog

### 🧱 Stack

`Node.js` · `Express` · `Stripe.js` · `HTML/CSS/JS` · `GitHub Actions`

### 📁 Structure

xplushop.luxfy/
├── index.html              # Your gaming storefront (preserved)
├── server.js               # Express server
├── api/
│   ├── create-checkout-session.js
│   └── webhook.js
├── src/
│   ├── catalog.js          # EDIT YOUR REAL PRICES HERE
│   └── stripe.js
├── public/js/stripe.js     # Browser helper: XplushopStripe.startCheckout()
├── docs/
├── .github/
├── terms.html / refund.html / privacy.html
└── CNAME (xplushop.xyz)
