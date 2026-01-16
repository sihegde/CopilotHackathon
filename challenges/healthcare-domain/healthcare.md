
#  Healthcare Appointment & Telemedicine Challenge 

---


## 🎯 Core Objective

Build a **minimal healthcare booking system** that supports:

✅ Role‑based access (Patient vs Doctor)  
✅ Appointment booking without conflicts  
✅ Doctor visibility into their schedule  
✅ Meaningful use of GitHub Copilot  

Optional features may be attempted **only after core tasks are stable**.

---

## 👥 Personas

### Patient
- Books an appointment (Virtual or In‑Person)
- Views their appointment details

### Doctor
- Views scheduled appointments for a day

---

## 🧠 Domain Constraints

Healthcare systems involve:
- Sensitive data
- Time‑based validation
- Strict access control

Your solution should **reflect these realities**, even in a simplified model.

---

## 📊 Model Data & Test Data 

Teams can use **CSV files as the source of truth**
- Load data into memory at runtime
- Apply business rules directly on this data


### 📁 Available CSV Files

The following CSVs are provided under: data folder.

### ⏰ Time Assumptions in Data

- All appointments are for **one day**: `2026-01-18`
- Appointment duration is **fixed at 15 minutes**
- Clinic working hours: **09:00 – 17:00**
- Appointments include:
  - Virtual and In‑Person visits
  - Cancelled entries
  - **Intentional overlapping bookings**

> 💡 The model data intentionally includes **invalid scenarios** so your logic can detect and handle them.

---

## 🧪 How the Data Is Expected to Be Used

Teams should decide how to:
- Load CSVs into memory
- Filter, validate, and transform the records
- Handle new bookings in memory (append / ignore / overwrite)
- Optionally write updated CSVs back to disk

There is **no prescribed approach** — this is part of the challenge.

---

## 1️⃣ Identity & Role‑Based Access

### Problem
Patients and Doctors must not access the same capabilities.

### Required Outcomes
- Two roles: **Patient** and **Doctor**
- Authentication (mocked or basic)
- At least one role‑restricted action

### Minimum Success
- Patient cannot access a doctor‑only view
- Doctor cannot access a patient‑only action

---

## 2️⃣ Appointment Booking Flow 

### Problem
Patients should book appointments without creating schedule conflicts.

### Required Outcomes
- Patient can request an appointment from available doctors
- Doctor can view their appointments for the day

### Constraints
- Use data from `appointments.csv`
- Fixed 30‑minute slots
- All logic applies to the **same calendar day**

### Minimum Success
- Overlapping bookings for the same doctor are **detected and prevented**
- Cancelled appointments are **ignored** when calculating availability

> 💡 The provided data is designed to test your overlap detection logic.

---

## 3️⃣ Quality Check

Healthcare systems demand reliability.

Choose **at least one**:
- ✅ Unit tests for appointment logic  
- ✅ Clear error handling & messages  
- ✅ Code refactoring for clarity  

### Minimum Success
- Demonstrate **intentional code quality improvement**

---

# 🌱 Optional Enhancements 

Attempt **only if mandatory tasks are complete**.

---

## Option A: Virtual Consultation (Optional)

- Associate consultation data with appointments
- Use `consultations.csv` for reference
- Mock video/chat acceptable

---

## Option B: Doctor Notes & Prescriptions

- Allow doctors to add notes to appointments
- Determine which fields patients can see

---

## Option C: Patient Health Records

- Aggregate past appointments and notes
- Provide patient‑only access

---



