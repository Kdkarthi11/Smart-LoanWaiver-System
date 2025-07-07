# Smart-LoanWaiver-System

A secure, full-stack web application designed to digitize and streamline the loan waiver process using biometric authentication, document validation, and real-time status tracking.  
The system supports both government administrators and individual applicants, ensuring transparency, security, and operational efficiency.

---

## 📌 Overview

**Smart-LoanWaiver-System** is a secure, full-stack web platform designed to automate loan waiver processing through biometric authentication, Aadhaar-based OCR, and real-time status tracking. It serves cooperative societies and government agencies by reducing fraud, manual errors, and delays in identity verification.

The system uses **EasyOCR** with a **Region of Interest (ROI)** approach to extract critical fields like **Name**, **Aadhaar ID**, **Smart Card ID**, and **Date of Birth** from uploaded documents. Facial recognition with **OpenCV** and **DeepFace** ensures live, biometric verification via webcam during onboarding and waiver checks.

Users authenticate using **OTP-based login** tied to their Aadhaar-linked mobile numbers. Admins verify document data, validate death certificates, apply eligibility rules, and update application status. All actions trigger real-time **email/SMS notifications** for transparency and security.

Built using **Python (Flask)** with a **MySQL backend** and a web interface developed in **VS Code** and **PyCharm**, the system is designed for scalable, multi-user environments and accessible from mobile or **e-Governance centers**.

**Core Workflow:**
- OTP-based login via Aadhaar-linked mobile number  
- Face recognition during account creation  
- OCR-based Aadhaar validation using EasyOCR  
- Admin-side loan eligibility verification and application review  
- Death certificate validation via document comparison with official records  
- Real-time email/SMS alerts on system activity and status updates

By combining traditional document processing with modern AI and computer vision, the system eliminates manual errors, enhances security, and increases operational efficiency.


## 🚀 Features

- ✅ **Role-Based Authentication**  
  Separate access flows for administrators and beneficiaries with secure dashboards.

- 🔐 **OTP-Based Aadhaar Login**  
  Login secured via OTP sent to Aadhaar-linked mobile numbers through integrated third-party APIs.

- 👤 **Biometric Face Recognition (OpenCV)**  
  Captures and authenticates facial data during onboarding and waiver processing to prevent identity fraud.

- 📄 **Aadhaar OCR Verification (EasyOCR + Regex)**  
  Extracts and validates Aadhaar details from uploaded documents to confirm user identity.

- 📊 **Loan Application & Status Tracking**  
  Users apply for loans and view real-time updates; admins review and manage loan applications.

- 🧠 **Liveness Detection (DeepFace)**  
  Detects whether the user is alive and matches stored facial data, preventing spoofing and ghost identity issues.

- ⚰️ **Deceased Verification for Loan Waiver**  
  Validates uploaded death certificates by comparing document info with a verified death registry before approving waivers.

- 🗃️ **Admin Dashboard**  
  Allows government officials to manage users, review submissions, and configure eligibility rules.

- 🧑‍🤝‍🧑 **Scalable MySQL Backend**  
  Structured database to support concurrent multi-user access with secure, normalized schema.

- 📬 **Intrusion Detection & Alerts**  
  Automatically detects suspicious login or identity misuse and sends instant notifications via email and SMS.

---

## 🛠️ Tech Stack

- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** Python (Flask)  
- **Database:** MySQL  
- **Libraries/Frameworks:** OpenCV, EasyOCR, DeepFace  
- **Authentication:** OTP API Integration  
- **Development Tools:** PyCharm, Visual Studio Code  
- **Testing Environment:** XAMPP (for local MySQL)
