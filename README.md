# veloura-pay
Veloura Pay — crypto-first checkout for digital products, with Telegram bot + instant delivery.

<p align="center">
  <img src="https://img.shields.io/badge/status-early%20development-yellow" alt="status" />
  <img src="https://img.shields.io/badge/build-passing-brightgreen" alt="build" />
  <img src="https://img.shields.io/badge/license-MIT-blue" alt="license" />
  <img src="https://img.shields.io/badge/payments-BTC%20Lightning%20%7C%20USDT-critical" alt="payments" />
  <img src="https://img.shields.io/badge/made%20with-%E2%9D%A4%EF%B8%8F%20in%20crypto-orange" alt="made with love" />
</p>

Veloura is a **crypto-first micro-commerce layer**: a Telegram bot and lightweight web checkout to sell digital goods (gift cards, mobile refills, eSIMs).  
Built for **crypto-friendly users worldwide**, with **multi-asset support** (BTC Lightning, USDT, and other popular options).

> Goal: instant purchase → on-chain confirmation → automated code delivery.

---

## Why
Crypto adoption is growing globally, and many users prefer crypto payments over traditional methods.  
Veloura provides a clean, reliable checkout and instant fulfillment experience.

## Core Features (MVP)
- Telegram bot + minimal web checkout
- Product catalog & pricing (via provider API)
- Crypto payments: **BTC Lightning / USDT** (extendable)
- Unique address per order, webhook confirmations
- Idempotent fulfillment + retries, instant code delivery

## Tech (initial)
- **Backend**: Node.js (Hono/Express), Cloudflare Workers
- **Storage**: Postgres/Supabase (`orders`, `products`, `deliveries`)
- **Bot**: Telegram Bot API
- **Payments**: on-chain listeners / provider webhooks

## Roadmap
- [ ] MVP: create orders, verify crypto payment, manual delivery
- [ ] Semi-auto: unique addresses + auto “paid” status
- [ ] Full-auto: provider API → code delivery in-chat
- [ ] Subscriptions & partner channels

## Safety & Reliability
- Idempotency keys for order calls
- Signed webhooks + audit logs
- Under/over-pay handling & refund paths

---

### Status
Early development. MVP targeted for pilot in crypto-friendly communities.

---

© 2025 Veloura. MIT License.
