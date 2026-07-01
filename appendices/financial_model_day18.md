# Financial Model Day 18 — NiBi AI

*File này là bản Markdown của Financial Model. Bạn có thể import vào Google Sheets hoặc Excel để nộp dưới dạng .xlsx*

---

## Sheet 1 — Assumptions

| Metric | Conservative | Base | Upside |
|---|---|---|---|
| Monthly itinerary users | 500 | 1.500 | 5.000 |
| Itinerary to lead rate | 10% | 15% | 20% |
| Qualified lead fee (VND) | 30.000 | 40.000 | 50.000 |
| Lead to booking rate | 10% | 15% | 25% |
| Average order value (VND) | 800.000 | 1.500.000 | 2.500.000 |
| Commission rate | 5% | 7% | 10% |

---

## Sheet 2 — Revenue Scenario

| Scenario | Users | Lead Rate | Qualified Leads | Revenue / Lead | Lead Revenue (VND) |
|---|---|---|---|---|---|
| **Conservative** | 500 | 10% | 50 | 30.000 | 1.500.000 |
| **Base** | 1.500 | 15% | 225 | 40.000 | 9.000.000 |
| **Upside** | 5.000 | 20% | 1.000 | 50.000 | 50.000.000 |

---

## Sheet 3 — Unit Economics

| Metric | Base Case |
|---|---|
| CAC per visitor | 8.000 VND |
| Visitor to itinerary completion | 50% |
| CAC per completed itinerary | 16.000 VND |
| Itinerary to qualified lead | 15% |
| CAC per qualified lead | ~106.667 VND |
| Revenue per qualified lead | 40.000 VND |
| **Insight** | Paid ads chưa hiệu quả nếu chưa tăng conversion hoặc revenue/lead |

---

## Sheet 4 — Cost & Payback

| Cost Item | Monthly Cost (VND) |
|---|---|
| Domain / hosting | 200.000 |
| AI API (LLM calls) | 500.000 |
| Data collection / cleaning | 1.000.000 |
| Content / SEO | 2.000.000 |
| Misc tools | 300.000 |
| **Total** | **4.000.000** |
