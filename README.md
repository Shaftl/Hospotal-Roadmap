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
# 🇦🇫 سیستم مدیریت شفاخانه‌های نسل نو — نسخه CodeArya

**سیستم هوشمند، مقیاس‌پذیر و انسانی برای کلینیک‌ها و شفاخانه‌های افغانستان**

یک اکوسیستم دیجیتال کامل برای خدمات صحی در افغانستان، طراحی‌شده با تمرکز بر **کار در حالت آفلاین**، **مقاومت در برابر انترنت ضعیف** و **هوش مصنوعی کمکی**.  
ساخته‌شده با **Next.js**, **Redux**, **Node.js**, **Express.js**, و **MongoDB** — ترکیبی از تجربهٔ کاربری مدرن و جریان کاری واقعی شفاخانه‌ها.

---

## 🩺 دیدگاه و فلسفه

> «تحول دیجیتال صحی باید انسانی، قابل اعتماد و به زبان مردم باشد.»

- مناسب برای شفاخانه‌های بزرگ و کلینیک‌های کوچک.
- بهینه‌شده برای محیط‌های دارای انترنت ضعیف (LAN محلی + همگام‌سازی ابری).
- رابط کاربری چندزبانه برای **دری، پشتو و انگلیسی**.
- ساده برای کارمندان تازه‌کار و قدرتمند برای مدیران.
- ساختار ماژولار و مقیاس‌پذیر با APIهای مدرن و کش هوشمند.

---

## 🧑‍⚕️ حساب‌ها و دسترسی‌ها

### ایجاد و مدیریت حساب‌ها

- ثبت‌نام توسط شماره تلفن یا ایمیل با **تأیید OTP** یا ایجاد توسط پذیرش.
- واردسازی گروهی اطلاعات از فایل Excel/CSV برای کارکنان و بیماران.
- حساب‌های موقتی برای کارمندان کوتاه‌مدت یا محصلان انترنی.

### نقش‌ها و صلاحیت‌ها

- نقش‌های اصلی: **مدیر، داکتر، نرس، پذیرش، داروفروش، لابراتوار، رادیولوژیست، حسابدار، مریض، پاک‌کار، امنیت، IT**.
- ساخت نقش‌های سفارشی با **دسترسی دقیق** برای هر ماژول (خواندن، ویرایش، چاپ).
- تقسیم صلاحیت بر اساس بخش (اطفال، جراحی، نسایی، عمومی).
- ارتباط میان بخش‌ها (داکتر ↔ لابراتوار ↔ داروخانه).

### امنیت و احراز هویت

- نشست‌ها بر اساس JWT + توکن تازه‌سازی.
- تأیید دو مرحله‌ای (SMS یا ایمیل).
- هشدار در صورت ورود از دستگاه جدید.
- بازنشانی رمز توسط SMS یا مدیر سیستم.
- مخفی‌سازی فیلدها بر اساس نقش (مثلاً بخش مالی یادداشت‌های کلینیکی را نمی‌بیند).

---

## 📊 داشبوردها و ناوبری

### داشبوردهای هوشمند

هر نقش یک داشبورد اختصاصی دارد با کارت‌های وضعیت و میانبرها.

| نقش | ویژگی‌های کلیدی |
| ---- | ---------------- |
| **مدیر** | نرخ اشغال بستر، درآمد امروز، هشدار موجودی، درخواست‌های در انتظار |
| **داکتر** | نوبت‌ها، نتایج لابراتوار، لیست مریضان، یادداشت‌های جدید |
| **نرس** | برنامه نوبت، علایم حیاتی، یادداشت انتقال شیفت |
| **پذیرش** | صف زنده، تقویم ملاقات، ثبت پرداخت |
| **داروفروش** | نسخه‌های در انتظار، موجودی پایین، تاریخ انقضا |
| **لابراتوار** | نمونه‌های جدید، نتایج آماده، آزمایش‌های فوری (STAT) |
| **مریض** | ملاقات‌ها، نسخه‌ها، فاکتورها، یادآوری پیگیری |

### ناوبری هوشمند

- جستجوی عمومی (`Ctrl + K`) برای مریض، آزمایش، فاکتور یا دارو.
- بخش «موارد اخیر» برای بازگشت سریع.
- کلیدهای میانبر برای کاربران حرفه‌ای.
- شاخص وضعیت آفلاین در رابط کاربری.

---

## 🧾 مدیریت مریضان و ویزیت‌ها

### ثبت مریض

- پروفایل کامل با **عکس، تذکره، اقارب، آلرژی‌ها، امراض مزمن**.
- ادغام خودکار سوابق تکراری.
- کارت مریض با QR/بارکد.
- مدیریت خانوادگی (تمام اعضا زیر یک سرپرست).

### نوبت و صف

- رزرو نوبت حضوری، تلفنی یا آنلاین.
- سیستم صف با نمایشگر شماره در انتظار.
- پیام SMS هنگام نزدیک شدن نوبت.
- تقویم حضور داکتران با رنگ‌بندی زمانی.

### بستری و رخصتی

- تخصیص بستر و بخش با تابلو زنده اشغال.
- انتقال بین بخش‌ها و روند رخصتی با تأیید مراحل.
- خلاصه رخصتی خودکار از EMR + فاکتور نهایی + نسخه.
- قابلیت «بستری مجدد» برای مریضان تکراری.

---

## 🩻 سیستم سوابق طبی (EMR)

### ویزیت و یادداشت

- قالب‌های SOAP برای ویزیت‌های مختلف (OPD، IPD، ER، ANC).
- لیست مشکلات، یادداشت درمان، و ضمیمه اسناد (PDF، عکس، اسکن).
- انتخاب تشخیص بر اساس کُدهای ICD-10 با جستجوی سریع.
- لینک ویزیت‌های پیگیری و نتایج.

### علایم حیاتی و گراف‌ها

- ثبت سریع (BP، HR، Temp، SpO₂، RR).
- نمودار روند با مناطق هشدار.
- هشدار خودکار برای علایم غیرعادی.
- پشتیبانی از دستگاه‌های بلوتوثی (در آینده).

### نسخه‌نویسی

- تولید نسخه الکترونیکی با بانک دارو و قالب‌های آماده.
- ارسال مستقیم به صف داروخانه.
- چاپ نسخه یا ارسال PDF.
- هشدار تداخل دارویی (در نسخه آینده).

---

## 🧪 لابراتوار و تصویربرداری

### لابراتوار

- ثبت و پیگیری آزمایش‌ها مستقیماً از EMR.
- رهگیری نمونه‌ها با بارکد یا QR.
- جریان وضعیت: **ثبت → جمع‌آوری → تحلیل → تأیید**.
- اطلاع‌رسانی خودکار SMS هنگام آماده شدن نتایج.

### رادیولوژی

- آپلود تصاویر و گزارش‌ها (X-Ray، CT، MRI، Ultrasound).
- نمایشگر تصاویر با ابزارهای بزرگ‌نمایی و توضیح.
- امضا و تأیید دیجیتال توسط رادیولوژیست.
- اتصال به PACS در فاز بعدی.

---

## 💊 داروخانه و ذخیره

### داروخانه

- صف نسخه‌ها با اولویت‌بندی.
- مدیریت دسته‌ها و تاریخ انقضا.
- محاسبه خودکار قیمت با تخفیف‌ها.
- اتصال مستقیم به صندوق پرداخت.

### ذخیره و تدارکات

- چند انبار (دارو، لابراتوار، عمومی، جراحی).
- هشدار موجودی پایین و درخواست خرید.
- مدیریت تأمین‌کنندگان و فاکتورهای خرید.
- تاریخچه کامل حرکات اجناس.

---

## 💰 بل و مالیات

### صورتحساب

- صدور فاکتور برای ویزیت، لابراتوار، دارو، و عملیات.
- پشتیبانی از پرداخت جزئی و بازپرداخت.
- رسید الکترونیکی (SMS یا ایمیل).
- عملکرد در حالت آفلاین.

### بیمه

- ثبت بیمه‌گرها و حد سقف پوشش.
- داشبورد ارسال ادعاهای بیمه.
- رهگیری وضعیت پرداخت و رد شدن.
- تقسیم پرداخت بین مریض و بیمه.

### گزارش‌های مالی

- خلاصه درآمد روزانه، بخش‌به‌بخش، و بدهی‌ها.
- خروجی به Excel یا PDF.
- سازگار با سیستم‌های حسابداری مانند QuickBooks.

---

## 📈 گزارش‌ها و تحلیل‌ها

### عملیاتی

- نرخ اشغال بستر، زمان انتظار، و عملکرد بخش‌ها.
- ارسال خودکار خلاصه روزانه به ایمیل مدیر.

### طبی

- تکرار تشخیص‌ها، روند نسخه‌ها، نتایج و مرگ‌ومیر.
- KPI داکتران و بخش‌ها.

### تحلیلی (AI در فاز بعدی)

- پیش‌بینی مریضان در معرض خطر.
- تحلیل مصرف دارو.
- شناسایی خستگی کارمندان.

---

## 📣 ارتباطات و اعلان‌ها

- پیام‌رسان داخلی بین کارمندان (داکتر ↔ نرس ↔ لاب ↔ داروخانه).
- اعلان از طریق SMS و ایمیل برای نوبت‌ها، نتایج، و پرداخت‌ها.
- هشدار صوتی (یکپارچه با Twilio یا شبکه محلی).
- اعلانات داخلی برای بخش‌ها و فوریت‌ها.

---

## 🧰 اسناد و فایل‌ها

- ذخیره مرکزی برای فایل‌ها و اسناد مریضان.
- برچسب‌گذاری بر اساس بخش یا نوع سند.
- نگهداری نسخه‌های مختلف گزارش‌ها.
- قالب‌های چاپی: نسخه، برچسب، گزارش، بند شناسایی.

---

## 👥 منابع بشری و نوبت‌کاری

- ثبت کارمندان با مدارک و گواهی‌ها.
- تنظیم نوبت‌ها با درگ-دراپ.
- مدیریت رخصتی و تأیید آنلاین.
- حضور با پین‌کد، RFID یا ورود مرورگر.
- صدور لیست معاشات (CSV, XLSX).

---

## 🔒 امنیت و محرمیت

- دسترسی بر اساس نقش‌ها (RBAC).
- محدودسازی دید در فیلدها.
- ثبت تمام فعالیت‌ها (ویرایش، حذف، مشاهده).
- رمزنگاری داده‌ها با AES-256.
- هاستینگ محلی برای نهادهای حساس.
- بک‌آپ خودکار و بازیابی فوری.

---

## 🌍 بومی‌سازی و دسترسی

- رابط چندزبانه (دری، پشتو، انگلیسی).
- پشتیبانی از RTL و LTR.
- کش آفلاین برای مناطق با انترنت ضعیف.
- حالت تاریک و روشن برای شیفت‌های شب.
- گفتار به نوشتار برای کارمندان نابینا (در آینده).
- طراحی ساده و آیکن‌محور برای آموزش سریع.

---

## ⚙️ تکنالوژی

| لایه | تکنالوژی |
| ---- | ---------- |
| Frontend | Next.js + Redux Toolkit + Tailwind + Shadcn/UI |
| Backend | Node.js + Express.js + MongoDB + Socket.IO |
| Auth | JWT + Refresh Token + 2FA |
| Cache | Redis یا IndexedDB |
| Reports | Mongo Aggregation + Recharts.js |
| Notifications | SMS Gateway (Roshan/Etisalat) + Nodemailer |
| Deployment | Docker + Nginx + PM2 |
| Offline Sync | Service Workers + Background Sync API |

---

## 🧠 هوش مصنوعی و اتوماسیون (آینده)

- **دستیار تریاژ:** تشخیص فوری بر اساس علایم حیاتی.
- **پیش‌بینی منابع انسانی:** پیشنهاد نوبت‌های کاری بهینه.
- **کدگذاری خودکار ICD-10 با NLP.**
- **پیش‌بینی ذخیره دارویی.**
- **چت‌بات مریضان برای نوبت‌دهی.**
- **تشخیص گفتار به متن برای داکتران.**

---

## 🖥️ استقرار و زیربنا

### حالت‌ها

1. **LAN محلی:** بدون انترنت با همگام‌سازی محلی.
2. **حالت ترکیبی:** LAN + همگام‌سازی شبانه ابری.
3. **حالت ابری:** برای شفاخانه‌های چند‌ شعبه‌ای.

### بک‌آپ و بازیابی

- بک‌آپ رمزنگاری‌شده روزانه (USB یا S3).
- بازیابی با یک کلیک.
- تأیید خودکار صحت بک‌آپ.

---

## 🔮 نقشه راه آینده

- اپلیکیشن موبایل (React Native/PWA).
- یکپارچگی با API وزارت صحت عامه.
- تله‌مدیسن (WebRTC).
- ورودی صوتی برای سوابق مریض.
- هشدار هوشمند وخامت وضعیت.
- سازگاری با HL7/FHIR.

---

## ❤️ ساخته‌شده برای افغانستان

- قابل اجرا در سخت‌افزار محلی حتی بدون انترنت.
- تمرکز بر **SMS به‌جای اپلیکیشن‌های پیچیده**.
- رابط ساده و شفاف به زبان مردم.
- طراحی زیبا و مقاوم بر اساس فلسفه CodeArya.

---

© 2025 **CodeArya Technologies** — تحول دیجیتال واقعی در خدمات صحی افغانستان 🇦🇫

