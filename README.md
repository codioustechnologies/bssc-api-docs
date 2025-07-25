# BSSC REST API

**Best Skin Specialist Chandigarh** – Secure Appointment Booking API

This repository contains the REST API code and OpenAPI (Swagger) documentation for managing doctor profiles, appointment availability, and patient bookings.

---

## 🔍 Overview

The BSSC API enables:

- 📋 Listing doctors with pagination
- 🔍 Viewing doctor profiles
- 📅 Checking availability by date
- ✅ Booking appointments securely
- 📨 Email notifications to users and admins
- ❌ Cancelling existing appointments
- 🩺 Fetching available medical specializations

All endpoints are RESTful and follow best practices for security, performance, and reliability.

---

## 🌐 API Base URL

https://bestskinspecialistchandigarh.com/wp-json/bsscapi/v1

---

## ⚙️ Available Endpoints

| Method | Endpoint                  | Description                        |
|--------|---------------------------|------------------------------------|
| GET    | `/doctors`                | List all doctors with pagination   |
| GET    | `/doctors/{id}`           | Get specific doctor by ID          |
| GET    | `/availability`           | Check doctor availability          |
| POST   | `/book`                   | Book an appointment (secured)      |
| GET    | `/bookings/{id}`          | View booking status by ID          |
| POST   | `/bookings/cancel`        | Cancel an appointment (secured)    |
| GET    | `/specializations`        | View medical specializations       |

> ⚠️ Secured endpoints require a valid nonce for access. For security reasons, the nonce generation route is not publicly listed here. Please contact admin for access.

---

## 📁 Swagger/OpenAPI Documentation

The complete OpenAPI 3.0 specification file is available in this repo as:

📄 bsscapi.yaml

You can:
- View it using [Swagger Editor](https://editor.swagger.io/)
- Or import into Postman / Swagger UI for testing

---

## 🛡️ Security

- Protected endpoints use WordPress nonces (`X-WP-Nonce` header)
- Only valid authenticated requests are allowed for appointment actions
- Nonces are generated per session and verified server-side
- Spam/fake entries are blocked via validations

---

## 🧪 Testing

- This API is built for production and used live at:
  
  👉 https://bestskinspecialistchandigarh.com

- Public access is restricted to prevent misuse.
- If you're a genuine partner or tester, request credentials or nonce access from the admin.

---

## 📜 License

This project is licensed under the **MIT License**.  
You are free to use and modify this API code for personal or commercial projects, but attribution is appreciated.

---

## 👨‍💻 Maintainer

**Best Skin Specialist Chandigarh**  
📧 info@bestskinspecialistchandigarh.com  
🌐 bestskinspecialistchandigarh.com

---

> This project is designed with care to support genuine appointment bookings for dermatologists and other medical specialists in Chandigarh and other. Abuse prevention and privacy are our top priorities.
