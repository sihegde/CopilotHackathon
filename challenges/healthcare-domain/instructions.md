
# 🏥 Healthcare Appointment & Telemedicine Challenge

## DESCRIPTION

The goal of this challenge is to build a **Healthcare Management Application** using the **pre‑provided healthcare dataset** available in this repository.


---

## AVAILABLE DATA

Healthcare domain data is already available in the following folder:
**challenges/healthcare-domain/data**

The dataset may include information related to:
- Patients
- Doctors / Healthcare Providers
- Appointments
- Medical records or visit information

---

## INSTRUCTIONS

1. **Choose a programming language and framework of your choice**
   - Backend, frontend, or full‑stack implementations are all acceptable.
   - You may build:
     - REST APIs
     - Web applications
     - CLI‑based applications

2. **Explore and Understand the Dataset**
   - Review the files in the `data` folder.
   - Identify:
     - Key entities
     - Relationships between entities
     - Required and optional fields
     - Data formats and constraints
   - Use **Copilot Chat** to:
     - Summarize dataset structure
     - Generate data models
     - Suggest validations and edge cases

3. **Design the Application Around the Existing Data**
   - Create APIs and UI workflows that align with the dataset.
   - Refer to Functional Requirements section to understand more and detailed steps.

---

## HINTS

- Start by asking Copilot:
  > “Analyze the healthcare dataset and explain the entities and relationships”
- Generate models **from the data**, not assumptions
- Let Copilot scaffold:
  - CRUD APIs
  - UI tables and detail screens
- Treat this challenge as a **real‑world data onboarding scenario**

---

## FUNCTIONAL REQUIREMENTS

### ✅ Backend / API (Data‑Driven)

Develop APIs that operate on the provided healthcare data.

#### Patient APIs
- Retrieve patient details by ID
- List patients with pagination or filters
- Update non‑sensitive patient information

#### Doctor / Provider APIs
- Retrieve doctor/provider details
- Search doctors by specialization, name, or availability
- List all healthcare providers

#### Appointment APIs
- Retrieve appointments by patient ID
- Retrieve appointments by provider ID
- Create a new appointment using existing entities
- Update appointment status (reschedule or cancel)

#### Medical Records APIs (if present in dataset)
- Retrieve medical history by patient ID
- View visit notes or prescriptions
- Associate records with appointments

---

### ✅ Frontend / UI (Web or CLI)

Create a UI that visualizes and interacts with real healthcare data:

- Dashboard displaying:
  - Patient summary
  - Upcoming appointments
- Views for:
  - Patient profile and medical history
  - Doctor/provider profile and schedule
  - Appointment details
- Forms to:
  - Book appointments
  - Update appointment status

(Optional)
- Search and filter:
  - Doctors by specialization
  - Appointments by date or patient
- Charts or summaries derived from the dataset

---

## NON‑FUNCTIONAL GUIDELINES

- Use **GitHub Copilot and Copilot Chat** extensively to:
  - Analyze the dataset
  - Scaffold APIs and controllers
  - Generate UI components
  - Refactor, document, and optimize code
- Ensure:
  - Clean separation of concerns
  - Readable and maintainable code
  - Graceful handling of invalid or missing data

---

## OPTIONAL EXTENSIONS

- Persist updates back to file or a database
- Add authentication and role‑based views (patient vs provider)
- Analytics dashboards:
  - Appointments per provider
  - Most common specializations
- Schema validation and data cleanup utilities

---



