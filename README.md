# 🇦🇫 Next-Gen Hospital Management System — CodeArya Edition

**Smart, Scalable, and Human-Centered Platform for Clinics & Hospitals in Afghanistan**

A complete digital healthcare ecosystem built for Afghan hospitals, designed with **low-bandwidth resilience**, **offline-first capability**, and **AI-assisted intelligence**.  
Built using **Next.js**, **Redux**, **Node.js**, **Express.js**, and **MongoDB** — blending modern UX with real-world hospital workflows.

---

## 🩺 Vision & Philosophy

> “Digital health that feels human, works offline, and speaks your language.”

- Designed for both large hospitals and small local clinics.
- Optimized for unstable internet — local LAN + cloud hybrid.
- Multilingual UI for **Dari**, **Pashto**, and **English**.
- Simple enough for first-time computer users; powerful enough for administrators.
- Structured to scale — modular micro-services, smart caching, and modern API design.

---

## 🧑‍⚕️ User Accounts & Access Control

### Account Creation & Management

- Self-registration via phone/email with **OTP verification** or reception onboarding.
- Bulk import (Excel/CSV) for staff and patient records.
- Temporary visitor accounts for short-term staff and interns.

### Roles & Permissions

- Built-in roles: **Admin**, **Doctor**, **Nurse**, **Reception**, **Pharmacist**, **Lab Tech**, **Radiologist**, **Accountant**, **Patient/Relative**, **Cleaner**, **Security**, **IT Support**.
- Custom role builder with **granular permissions** (view/edit/export per module).
- Department-based scoping (e.g. Pediatrics, Surgery, Maternity).
- Cross-department access rules (Doctors ↔ Lab ↔ Pharmacy).

### Authentication & Security

- JWT-based sessions + Refresh tokens.
- Two-Factor Authentication (SMS/Email OTP).
- Device fingerprinting (alerts when login from new device).
- Password reset via SMS or secure admin override.
- Role-based field masking (finance cannot see clinical notes, etc.).

---

## 📊 Dashboards & Navigation

### Adaptive Dashboards

Each user gets a **role-specific dashboard** with quick-action cards, metrics, and shortcuts.

| Role           | Key Highlights                                                     |
| -------------- | ------------------------------------------------------------------ |
| **Admin**      | Occupancy rate, revenue today, inventory alerts, pending approvals |
| **Doctor**     | Appointments, pending labs, patient list, unread notes             |
| **Nurse**      | Ward schedule, vitals due, shift handovers                         |
| **Reception**  | Queue, appointment calendar, check-ins, payments                   |
| **Pharmacist** | Prescription queue, low stock, batch expiry                        |
| **Lab Tech**   | Sample queue, result validation, STAT requests                     |
| **Patient**    | Visits, prescriptions, invoices, follow-up reminders               |

### Smart Navigation

- Global search bar (`Ctrl + K`) for patients, labs, invoices, or drugs.
- “Recent items” sidebar for quick recall.
- Keyboard shortcuts for power users.
- Offline mode indicator (sync status shown in UI).

---

## 🧾 Patient & Visit Management

### Patient Registry

- Profile with **photo**, **Tazkira/National ID**, **family link**, allergies, and chronic diseases.
- Smart merge for duplicate records.
- QR/Barcode patient ID cards (printable).
- Household view — manage entire family profiles under one guardian.

### Appointment & Queue

- Hybrid booking (walk-in, phone, online).
- Ticket/number display board for waiting area.
- Real-time queue status with SMS notification when turn approaches.
- Doctor availability calendar with color-coded time slots.

### Admission & Discharge

- Bed & ward allocation, live occupancy board.
- Transfer and discharge workflows with approval steps.
- Discharge summary auto-generated from EMR + final bill + prescription.
- “Readmit” shortcut for repeat cases.

---

## 🩻 Electronic Medical Records (EMR)

### Encounter Management

- SOAP format templates, reusable visit types (OPD, IPD, ER, ANC, Surgery).
- Problem lists, treatment notes, and attachments (PDF, images, scans).
- Tagging by ICD-10 codes with autosuggest search.
- Linked follow-up notes and outcomes.

### Vitals & Charts

- Quick vitals capture (BP, HR, Temp, SpO₂, RR).
- Trend charts with warning color zones.
- Auto-flag abnormal vitals and notify nurse in charge.
- Integration with Bluetooth devices (future phase).

### Prescriptions

- E-Prescription generator with drug database, dosage templates, and refills.
- Send directly to pharmacy queue.
- Generate patient copy (print/PDF).
- Drug interaction warnings (AI-based future enhancement).

---

## 🧪 Laboratory & Imaging

### Lab Management

- Create, collect, and track lab orders directly from EMR.
- Sample tracking via barcode or QR labels.
- Status workflow: **Ordered → Collected → Analyzing → Approved**.
- Auto SMS notification when results ready.

### Radiology

- Upload images or reports (X-ray, CT, MRI, Ultrasound).
- Viewer with annotations & contrast adjustment.
- Radiologist approval + digital signature.
- Integration with PACS (Phase 2).

---

## 💊 Pharmacy & Inventory Management

### Pharmacy Module

- Live prescription queue with priority flags.
- Batch & expiry management, controlled substance logs.
- Auto price calculation with markup/discount policies.
- Quick billing integration with cashier counter.

### Inventory Module

- Multi-store (pharmacy, lab, general, OT).
- Reorder alerts and purchase requests.
- Supplier management + purchase order tracking.
- Full audit trail of stock movements.

---

## 💰 Billing, Finance & Insurance

### Core Billing

- Create bills for visits, labs, pharmacy, and procedures.
- Support for **partial payments**, **refunds**, and **credit mode**.
- Instant SMS/e-receipt generation.
- Offline billing for network-down mode.

### Insurance & Contracts

- Maintain payer list with coverage limits.
- Claim submission dashboard.
- Claim tracking + rejection reason logging.
- Patient/Insurer split billing with visual breakdown.

### Finance Reports

- Daily income sheet, revenue by department, expense summary.
- Unpaid invoices and aging report.
- Export to Excel, PDF, or QuickBooks format.

---

## 📈 Reports & Analytics

### Operational Insights

- Bed occupancy rate, turnover time, and wait time analysis.
- Department-wise performance dashboards.
- Auto email daily summary to admin.

### Clinical Analytics

- Disease frequency, patient outcomes, prescription trends.
- Mortality/morbidity logs with filters.
- Doctor performance KPIs.

### Predictive AI Reports (Phase 2)

- Early detection of high-risk patients (based on vitals & visits).
- Forecasting medicine consumption.
- Attendance & staff fatigue prediction.

---

## 📣 Communication & Alerts

- Built-in chat for care coordination (doctor↔nurse↔lab↔pharmacy).
- SMS/Email notifications: appointments, lab ready, billing, reminders.
- Voice call alert integration (Twilio/local gateway ready).
- In-app announcements for policy changes or emergencies.

---

## 🧰 Document & File Management

- Centralized media library for patient documents and scans.
- Tagging and quick filtering by patient, department, or type.
- Version control for critical documents (lab reports, consent forms).
- Printable templates (prescriptions, labels, reports, ID bands).

---

## 👥 HR & Workforce Management

- Staff registry with documents and certifications.
- Shift scheduler with drag-drop UI.
- Leave management and approval flow.
- Attendance tracking via pin, RFID, or browser login.
- Payroll export (CSV, XLSX, or API integration).

---

## 🔒 Security, Privacy & Compliance

- Role-based access control (RBAC).
- Field-level access restriction.
- Full **audit logs** for edit/delete/view actions.
- Data encryption (AES-256) for backups.
- Local-only hosting option for sensitive hospitals.
- Auto backup + one-click restore system.

---

## 🌍 Localization & Accessibility

- Multilingual (Dari / Pashto / English).
- RTL and LTR layout support.
- Offline caching for poor internet areas.
- Dark & high-contrast mode for night shifts.
- Text-to-speech (for visually impaired staff, Phase 2).
- Simple, icon-driven UI for minimal training.

---

## ⚙️ Technology Stack Overview

| Layer         | Technology                                                  |
| ------------- | ----------------------------------------------------------- |
| Frontend      | Next.js (App Router) + Redux Toolkit + Tailwind + Shadcn/UI |
| Backend       | Node.js + Express.js + MongoDB + Socket.IO                  |
| Auth          | JWT + Refresh Token + 2FA (SMS/Email)                       |
| Caching       | Redis or IndexedDB (offline mode)                           |
| Reports       | Mongo Aggregation + Recharts.js                             |
| Notifications | SMS Gateway (Roshan, Etisalat) + Nodemailer                 |
| Deployment    | Docker + Nginx + PM2                                        |
| Offline Sync  | Service Workers + Background Sync API                       |

---

## 🧠 AI & Automation Layer (Future Enhancements)

- **AI Triage Assistant:** auto-classify urgency based on vitals & symptoms.
- **Predictive Staffing:** suggest staffing levels per department.
- **Auto ICD-10 coding** via NLP on encounter notes.
- **AI Inventory Forecast:** predict shortages and reorder times.
- **Chatbot Triage (Patient Portal):** symptom-based triage with appointment booking.
- **Voice Note Recognition:** doctors dictate notes, system converts to EMR text.

---

## 🖥️ Deployment & Infrastructure

### Deployment Modes

1. **Local LAN Mode:** works without internet, uses local IP sync.
2. **Hybrid Mode:** LAN + nightly sync to cloud backup.
3. **Cloud Mode:** centralized for multi-branch hospitals.

### Backup & Restore

- Daily encrypted backup to USB or S3.
- One-click restore wizard.
- Auto verify backup integrity.

---

## 🔮 Future Roadmap

- **Mobile App (React Native/PWA)** for doctors & patients.
- **Government Health API Integration** (for national reporting).
- **Telemedicine (WebRTC)** with appointment sync.
- **Voice-based Patient Record Entry.**
- **AI-based Deterioration Alerts.**
- **HL7/FHIR interoperability layer.**

---

## ❤️ Built for Afghanistan

- Runs on local hardware, even offline.
- SMS first, app second — usable by feature phones.
- Clear Dari/Pashto interface.
- Visual, icon-based layout for quick learning.
- Backed by CodeArya’s design philosophy: _practical, beautiful, resilient._

---

© 2025 **CodeArya Technologies** — Empowering Afghan Healthcare with Modern, Human Technology 🇦🇫
