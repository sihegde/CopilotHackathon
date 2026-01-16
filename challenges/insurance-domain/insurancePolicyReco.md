
# Insurance — Policy Recommendation & Eligibility Engine 

---

## 🎯 Core Objective

Build a **minimal service** that:

✅ Accepts customer profile and preferences  
✅ Evaluates **eligibility** against policies  
✅ Recommends **suitable policies**  
✅ **Explains** why a policy was recommended or rejected

---

## 👥 Personas

- **Customer:** provides profile + preferences  
- **Advisor (optional):** reviews engine output

---

## 🧠 Domain Constraints

- Policies have **age**, **risk**, **budget**, and **smoker** constraints.
- Recommendations should **explain** both **why included** and **why excluded**.  
- No database—**CSV files** are the source of truth.

---

## 📊 Model Data (CSV)

All data is provided as CSVs. Load into memory and apply rules.

Placed in: `data`

- `policies.csv` — available policies with constraints  
- `customers.csv` — sample customers  
- `preferences.csv` — customer preferences (budget, category, coverage)  
- `eligibility_rules.csv` — plain-English rule descriptions  
- `expected_samples.csv` — (optional) examples to sanity-check your output format

**Timebox hint:** You may work with **one customer at a time** (e.g., `CUS-001`) to keep scope tight.

---

## ✅ Mandatory Tasks

### 1) Input & Validation
- Accept a **customer_id** and read their profile + preferences from CSV.
- Validate required fields and reasonable ranges (age, budget, risk).

### 2) Eligibility Evaluation
- For each policy, decide **Eligible / Ineligible**:
  - Consider age, risk score, smoker rules, preexisting condition wait, budget, category, sum insured.
- Capture **explanations per policy** listing **passed/failed rules**.

### 3) Recommendations
- From **eligible** policies, rank top matches (you decide the logic—e.g., budget fit + higher sum insured).
- Return results with a simple justification and show **why top 1–3 were chosen**.

### Minimum Success Criteria
- A clear API/CLI endpoint that returns:
  - Customer context (basic)
  - Eligible policies with reasons
  - Ineligible policies with reasons
  - Final top recommendations (1–3) with concise explanations

---

## 🌱 Optional Enhancements (Stretch)

- **Tunable Scoring:** add weighted scoring (budget fit, sum insured, age closeness).  
- **Fallback Recommendations:** when no eligible policy found in preferred category, suggest **nearest category** with a disclaimer.  
- **What‑If Simulation:** allow tweaking budget/risk to see how recommendations shift.  
- **Audit Report:** generate a compact “decision explanation log” (JSON or text).

---
