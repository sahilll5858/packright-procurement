# 📦 PacketRight Manufacturing · Vendor Comparison & Procurement Assistant

A **single-file, static, deploy-anywhere** capstone (Topic 04: *Vendor Comparison
and Procurement Assistant*) for the "Gen AI for Business" programme.

It helps a fictional manufacturing company buy **corrugated cartons & packaging
materials** more transparently:

1. **Three fictional quotations arrive in inconsistent formats** — INR all-inclusive,
   USD + freight + IGST, and ex-works with GST extra.
2. The browser **standardises** them into one table (landed-cost INR incl. GST +
   freight, lead-time days, burst-strength grade 0–10).
3. Vendors are **compared** on four weighted criteria you edit live (Quality,
   Cost, Lead Time, Reliability).
4. A **policy check** flags any vendor below the minimum strength grade as
   Non-Compliant and excludes it from the recommendation — price never overrides safety.
5. The system **recommends** one vendor, and a human **reviews / overrides** it.
6. **No autonomous purchasing**: the tool only records a **draft** approval for Finance.

## ✅ Why this needs no backend, no Docker, no API keys

Everything runs inside the browser (`index.html`):

- Weighted scoring & recommendation — pure deterministic JavaScript (reproducible).
- Policy knowledge base & Q&A — disclosed rule-based assistant (swap for an LLM in production).
- PDF quotation reading — client-side via `pdf.js` from a CDN (nothing is uploaded).
- Approval history — stored in the browser's `localStorage`.
- $0 running cost — just static files.

## 📂 Files

```
index.html      # the entire app (HTML + CSS + JS)
README.md       # this file
```

No build step, no package manager, no server.

## 🚀 Deploy for free (⭐ pick one)

### 1. GitHub Pages (recommended)
1. Create a repo → push `index.html` (e.g. to branch `main`).
2. Repo → **Settings → Pages → Build and deployment → Source: Deploy from a branch → main / (root)** → Save.
3. Your site is live at `https://<username>.github.io/<repo>/` in a minute.

### 2. Netlify Drop (fastest, no git)
1. Go to https://app.netlify.com/drop
2. Drag-and-drop the folder containing `index.html`.
3. You get a public `*.netlify.app` URL instantly.

### 3. Vercel
1. Push to GitHub, import the repo in https://vercel.com
2. Framework preset: **Other** → Deploy. Static site only, no config.

## 🖥️ Run locally (optional)
Just double-click `index.html`, or serve it:

```bash
npx serve .
```

## 🎯 Minimum-viable capstone covered
- One purchasing category (cartons & packaging) ✔
- Three fictional quotations, standardised ✔
- Comparison on learner-chosen criteria ✔
- Reviewable recommendation ✔
- Human-in-the-loop override + approval history ✔
- Explains decision criteria, and the system never makes purchases/commitments independently ✔

## 🔒 Safety statement
This assistant produces a transparent, overrideable **recommendation only**. It
executes no purchase, no payment and no contractual commitment on its own. The
final signing authority always rests with authorised PackRight Manufacturing
personnel.