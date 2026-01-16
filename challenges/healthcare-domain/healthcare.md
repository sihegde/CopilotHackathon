## Healthcare Appointment & Telemedicine Challenge

---

## 🎯 Core Challenge Objective

Build a **minimal healthcare platform** that demonstrates:

✅ Role‑based access (Patient & Doctor)  
✅ Appointment booking without conflicts  
✅ Doctor visibility into scheduled appointments  
✅ Thoughtful use of GitHub Copilot  

Optional features may be attempted **only after mandatory tasks are stable**.

---

## 👥 Personas

### Patient
- Books an appointment (Virtual or In‑Person)
- Views their booking details

### Doctor
- Views scheduled appointments
- May participate in consultations (optional)

---

## 🧠 Domain Context

Healthcare systems have:
- **Sensitive data**
- **Time‑critical flows**
- **Strict access requirements**

Your design choices should reflect these realities, even in a simplified form.

---

# ✅ Mandatory Tasks


## 1️⃣ Identity & Role-Based Access 
### Problem
Patients and Doctors should not access the same capabilities.

### Required Outcomes
- Two distinct roles: **Patient** and **Doctor**
- Authentication (can be mocked or basic)
- At least one route or feature protected by role

### Minimum Success Criteria
- A patient-only feature that a doctor **cannot** access
- A doctor-only feature that a patient **cannot** access

### Design Considerations
- How are roles stored and verified?
- Where is access enforced—frontend, backend, or both?
- What data should never be exposed?


---

## 2️⃣ Appointment Booking Flow 

### Problem
Patients must be able to book time with doctors without clashes.

### Required Outcomes
- Patient can book an appointment:
  - Type: Virtual or In‑Person
- Doctor can view their scheduled appointments

### Constraints 
- Only **one day** of appointments
- Fixed duration per appointment (e.g., 15 minutes)

### Minimum Success Criteria
- Overlapping bookings are **prevented**
- System clearly shows booking success or failure

### Design Considerations
- How do you represent time?
- How do you detect conflicts?
- What happens when an appointment is cancelled?


---

## 3️⃣ Quality Check

Healthcare systems require trust and reliability.

### Choose **at least ONE**:
- ✅ Add unit tests for booking logic  
- ✅ Implement meaningful error handling  
- ✅ Refactor logic for readability and maintainability  

### Minimum Success Criteria
- Demonstrate **intentional improvement** to code quality


---

# 🌱 Optional Enhancements (Stretch Goals)

---

## Option A: Virtual Consultation

- Link online consultation to an appointment
- Mock video call OR simple text chat between doctor and patient

Think about:
- Who can join a consultation?
- When does it start and end?

---

## Option B: Doctor Notes & Prescriptions

- Allow doctors to add notes to appointments
- Allow patients to view permitted notes

Think about:
- Private vs shared notes
- Long‑term record keeping

---

## Option C: Patient Health Records 

- Maintain basic patient history
- Allow patients to view/download records

Think about:
- Privacy
- Access control
- Data ownership

---


