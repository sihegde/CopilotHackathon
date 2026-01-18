
# 🛡️ Insurance Management Application Challenge

## DESCRIPTION

The goal of this challenge is to build an **Insurance Management Application** using the **pre‑provided insurance dataset** available in this repository.

---

## AVAILABLE DATA

Insurance domain data is already available in the following folder:
**challenges/insurance-domain/data**

The dataset may include information related to:
- Customers / Policyholders
- Insurance Policies
- Claims
- Premium payments
- Coverage details

---

## INSTRUCTIONS

1. **Choose a programming language and framework of your choice**
   - Backend, frontend, or full‑stack implementations are all acceptable.
   - You may build:
     - REST APIs
     - Web applications
     - CLI‑based applications

2. **Explore and Understand the Dataset**
   - Review files in the `data` folder.
   - Identify:
     - Key entities (customers, policies, claims, payments)
     - Relationships between entities
     - Required and optional attributes
     - Status fields and lifecycle states
   - Use **Copilot Chat** to:
     - Summarize dataset structure
     - Generate domain models
     - Propose validations and constraints

3. **Design the Application Around the Existing Data**
   - APIs and UI flows should reflect real insurance processes.
   - Avoid altering data semantics unless implementing optional extensions.

---

## HINTS

- Start by asking Copilot:

> “Analyze the insurance dataset and explain customers, policies, and claims relationships”

- Let the data drive your domain design
- Use Copilot to quickly scaffold CRUD operations and dashboards
- Treat this as an enterprise insurance system onboarding exercise

---

## FUNCTIONAL REQUIREMENTS

### ✅ Backend / API (Data‑Driven)

Develop APIs that operate directly on the provided insurance dataset.

#### Customer / Policyholder APIs
- Retrieve customer details by ID
- List customers with filtering or pagination
- Update customer contact information

#### Policy APIs
- Retrieve policy details by policy number
- List policies by customer ID
- View coverage details and policy status
- Create or renew policies (if supported by dataset)

#### Claims APIs
- Retrieve claims by policy ID or customer ID
- Create a new claim using existing policy data
- Update claim status (submitted, under review, approved, rejected)
- View claim history and claim amounts

#### Payment APIs (if present in dataset)
- Retrieve premium payment history
- View outstanding or overdue payments
- Associate payments with policies

---

### ✅ Frontend / UI (Web or CLI)

Build a UI that visualizes and interacts with real insurance data:

- Dashboard showing:
  - Active policies
  - Recent claims
  - Payment status alerts
- Screens for:
  - Customer profile
  - Policy details and coverage
  - Claim details and claim lifecycle
- Forms to:
  - File a new claim
  - Update customer information

(Optional)
- Search and filter:
  - Policies by status or type
  - Claims by status or date
- Data summaries or charts:
  - Claims per policy
  - Premiums per customer

---

## NON‑FUNCTIONAL GUIDELINES

- Use **GitHub Copilot and Copilot Chat** extensively to:
  - Analyze the dataset
  - Scaffold controllers, services, and models
  - Generate UI components
  - Document and refactor logic
- Ensure:
  - Clean separation of concerns
  - Clear naming aligned to insurance terminology
  - Graceful handling of missing or invalid data

---

## OPTIONAL EXTENSIONS

- Persist updates back to file or database
- Add role‑based access (customer, agent, admin)
- Claims analytics dashboard
- Policy renewal reminders
- Fraud detection heuristics using claims data

---


