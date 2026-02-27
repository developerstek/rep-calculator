# 📄 Replit Invoice Cost Calculator

A browser-based tool that parses Replit invoice PDFs and aggregates costs by Billing ID, Month, and Category — no server or install required.

## 🚀 Usage

1. Open `index.html` in Chrome or Safari
2. **Drop or browse** your Replit invoice PDF(s) — single or bulk
3. Click **⚡ Parse & Calculate**
4. Explore results across 4 tabs

## 📊 Views

| Tab | Description |
|-----|-------------|
| 🆔 By Billing ID | All billing IDs with total cost, active categories, and months |
| 📅 By Month | Costs grouped by invoice month, sorted by amount |
| 🏷️ By Category | Service categories (Agent Usage, Autoscale, Neon Compute, etc.) with per-ID cost + % share |
| ⊞ Month × ID Pivot | Cross-table showing every billing ID vs every month |

## 🔍 Features

- **Click any Billing ID** → opens a detail modal with category + month breakdown
- **Search** billing IDs in real-time
- **Sort** by amount (high/low), alphabetical, or category count
- **Export CSV** — available for each view

## 📁 Invoice Format

Designed for **Replit** invoices containing:
- Billing IDs in UUID format (e.g. `3241ad86-6089-4fb8-abf1-d930bd90ac2a`)
- Categories: Agent Usage, Autoscale Deployments, Autoscale Requests, Deployments Outbound Data Transfer, Neon Compute Time

## ⚙️ Technical

- **Pure HTML + JavaScript** — no install, no backend, no dependencies to manage
- Uses [PDF.js](https://mozilla.github.io/pdf.js/) (loaded from CDN) for client-side PDF parsing
- All data stays in your browser — nothing is uploaded anywhere
