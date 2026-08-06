# 📦 PackRight Manufacturing · Vendor Comparison & Procurement Assistant

A **single-file, static, deploy-anywhere** capstone (**Topic 04 — Vendor Comparison
and Procurement Assistant**) for the "Gen AI for Business" programme.

It helps a fictional manufacturing company buy **corrugated cartons & packaging
materials** more transparently:

1. **Three fictional quotations arrive in inconsistent formats** — INR all-inclusive,
   USD + freight + IGST, and ex-works with GST extra.
2. The browser **standardises** them into one table (landed-cost INR incl. GST +
   freight, lead-time days, burst-strength grade 0–10).
3. Vendors are **compared** on four weighted criteria you edit live (Quality,
   Cost, Lead Time, Reliability).
4. A **policy check** flags any vendor below the minimum strength grade as
   Non-Compliant and excludes it — price never overrides quality.
5. The system **recommends** one vendor with explainable reasoning, and a human
   **reviews / overrides** it (What‑if sensitivity included).
6. **No autonomous purchasing**: the tool only records a **draft** approval for Finance.

## ✅ Why it needs no backend, no Docker, no API keys
Everything runs in `index.html`:
- Weighted scoring & recommendation — deterministic (auditable, reproducible).
- Policy Q&A — disclosed rule-based assistant (LLM-pluggable for production).
- PDF quotation reading — client-side via `pdf.js` (nothing is uploaded).
- Approval history & email drafts — `localStorage` + `mailto:`, no server.
- $0 running cost — plain static files.

## 📁 Deliverables
| File | Purpose |
|------|---------|
| `index.html` | The entire web app (HTML + CSS + JS) |
| `README.md` | This guide |
| `SUBMISSION_FORMAT.md` | 8-field submission table (name, roll no, description, problem, tools, outcomes, link) |
| `DEMO_SCRIPT.md` | Step-by-step script for the final demonstration |
| `Project_Overview.pptx` | 3-slide submission deck |
| `Project_Overview.pdf` | 3-page overview (print-friendly) |
| `assets/screenshots/` | Screenshots of all 8 tabs of the live app |

## 🚀 Deploy for free (pick one)
### 1. GitHub Pages (in use)
1. Push `index.html` (and docs) to a repo on branch `main`.
2. Repo → Settings → Pages → Source: Deploy from branch → `main / (root)` → Save.
3. Live at `https://<user>.github.io/<repo>/`.

### 2. Netlify Drop
Drag the folder containing `index.html` onto https://app.netlify.com/drop → get a `*.netlify.app` URL.

### 3. Vercel
Import the repo → Framework preset: Other → Deploy.

## 🖥️ Run locally
Double-click `index.html`, or `npx serve .`

## 🎯 Minimum-viable capstone covered
- One purchasing category (cartons & packaging) ✔
- Three fictional quotations, standardised ✔
- Comparison on learner-chosen criteria ✔
- Reviewable recommendation + human-in-the-loop override ✔
- Approval history, explainable scoring, sensitivity analysis ✔
- Never makes purchases/commitments independently ✔

## 🔒 Safety statement
This assistant produces a transparent, overrideable **recommendation only**. It
executes no purchase, no payment and no contractual commitment on its own. The
final signing authority always rests with authorised PackRight personnel.