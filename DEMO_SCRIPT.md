# Final Demonstration Script

**Project:** Malpani Group — Vendor Comparison & Procurement Assistant
**Scenario:** Buying **10,000 heavy-duty corrugated cartons** (Corrugated Cartons & Packaging Materials)
**Live URL:** https://sahilll5858.github.io/packright-procurement/

---

## 1. The problem (30s)
*"Our procurement team receives carton quotations in completely different formats — one vendor quotes INR all-inclusive, another quotes USD with freight on top, and a third quotes ex-works without GST. Comparing them manually takes hours and is error-prone."*

## 2. The three vendors (fictional)
| Vendor | How the quote arrived |
|--------|------------------------|
| CorrLite Packaging | INR all-inclusive, 5 days, Grade A, recyclable kraft |
| EuroCarton Works | **USD 6,600 + IGST 18%**, 18 days, Grade A+ (imported) |
| PackDesk Supplies | **Ex-works, GST extra**, 8 days, Grade B (below spec) |

## 3. The standardisation
Open **Tab 3 — Standardised comparison**.
*"The assistant normalises everything to one yardstick: landed-cost INR (incl. GST + freight), lead time in days, and a burst-strength grade out of 10."*
Call out: EuroCarton's USD price converted at a fixed budget rate (1 USD = 84 INR); PackDesk's ex-works price had GST added.

## 4. The decision criteria (explain WHY)
Sidebar weights (editable live):
- **Quality / strength 40%** — burst resistance is non-negotiable for our line.
- **Lead Time 25%** — the packaging line cannot wait for cartons.
- **Cost 25%** — landed INR for a fair like-for-like.
- **Reliability 10%** — on-time delivery history.
*"Weights are live in the sidebar, so we can demonstrate sensitivity."*

## 5. The recommendation + policy
- **PackDesk Supplies** fails the **≥ 8 strength policy** → flagged 🚫 and **excluded**, no matter how cheap.
- Recommended = **CorrLite Packaging** (score **95.5/100**): best compliant, 5-day lead, recyclable mill, and near-lowest landed cost.
- *"The sub-spec vendor never overrides quality."*
- **Try it:** raise the **Green bonus** → shows the sustainability uplift live.

## 6. Explainable reasoning + what-if
Open **Tab 5 — Review & approve**.
- Show the **"Why this vendor?"** matrix: per-criterion sub-scores for all vendors.
- Show the **sensitivity note**: *"Raising the Cost weight to ~43% would flip the recommendation to EuroCarton."*
- *"Every number is reproducible — no hidden AI in the scoring."*

## 7. Human-in-the-loop (the key requirement)
Still on Tab 5:
- Show the recommended vendor pre-selected.
- **Override** to a different vendor → add a justification.
- Click **"Record decision (draft only)"**.
*Call-out:* *"This only records intent for Finance. It does not place an order, sign anything, or move money."*
- Show the **Approval history** table.

## 8. Extras (time permitting)
- **Tab 6 — Policy assistant**: *"What strength grade must vendors meet?"*
- **Tab 7 — Email vendor**: draft an **RFQ** / clarification mail to a vendor (mailto).
- **Tab 8 — Extras**: upload a quotation **PDF** → parsed client-side; paste raw quote text → standardise.

## 9. Closing safety message
*"This tool is transparent and overrideable, and it never commits funds. The final sign-off physically lives with authorised Malpani Group personnel."*

---

## What the final demonstration must show (guideline mapping)
- ✅ Original business information → raw quotations (Tab 2)
- ✅ The insight produced → standardised comparison + scores (Tab 3)
- ✅ The action from that insight → recommendation (Tab 5)
- ✅ How a user reviews/uses the output → review, override, approval history (Tab 5)
- ✅ Which business metric could improve → quotation-to-decision time, hidden-cost reduction, zero non-compliant awards (Tab 1 / discussion)