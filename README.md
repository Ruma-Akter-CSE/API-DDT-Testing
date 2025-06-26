# API-DDT-Testing

# API Booking Automation Project

This project involves automated API testing of a booking system using **Postman** and **Newman**. It covers key functionalities like creating, reading, updating, and deleting bookings, as well as authentication and data-driven testing (DDT).

---

## 📊 Newman Report Summary

**Collection Name:** `Booking_collection`  
**Execution Time:** Wed Jun 25 2025, 23:50 (BST)  
**Exported With:** Newman v6.2.1

| Metric                  | Value           |
|------------------------|-----------------|
| Total Iterations       | 10              |
| Total Requests         | 50              |
| Pre-request Scripts    | 10              |
| Test Scripts           | 30              |
| Assertions             | 71              |
| Total Duration         | 3.4s            |
| Avg. Response Time     | 541ms           |
| Total Data Received    | 576B (approx)   |
| Total Failures         | 1               |

---

## ✅ Request Summary

### 1. `Create_booking` (POST)
- **URL:** `https://restful-booker.herokuapp.com/booking/`
- **Status Code:** 200
- **Mean Time:** 1717ms
- **Tests Passed/Failed:** 0 / 0

---

### 2. `Get_Booking` (GET)
- **URL:** `https://restful-booker.herokuapp.com/booking/6573`
- **Status Code:** 200
- **Mean Time:** 253ms
- **Tests Passed/Failed:** 6 / 1

**Tests:**

| Test Name              | Pass | Fail |
|------------------------|------|------|
| first name variable    | ✅   |      |
| last name variable     | ✅   |      |
| totalprice variable    | ✅   |      |
| depositpaid variable   |      | ❌   |
| additionalneeds        | ✅   |      |
| checkin variable       | ✅   |      |
| checkout variable      | ✅   |      |

❗ **Failure Reason:**  
`AssertionError: depositpaid variable — expected 'true' to deeply equal true`

---

### 3. `Create_token` (POST)
- **URL:** `https://restful-booker.herokuapp.com/auth`
- **Status Code:** 200
- **Tests Passed/Failed:** 0 / 0

---

### 4. `Update_booking` (PUT)
- **URL:** `https://restful-booker.herokuapp.com/booking/6573`
- **Status Code:** 200
- **Tests Passed/Failed:** 0 / 0

---

### 5. `Delete_booking` (DELETE)
- **URL:** `https://restful-booker.herokuapp.com/booking/1046`
- **Status Code:** 201
- **Tests Passed/Failed:** 0 / 0

---

## 🧪 Tools Used
- Postman
- Newman
- JavaScript (for test scripts)
- Data-driven testing using CSV/JSON

---

## 📌 Note
This project validates booking APIs including all CRUD operations and token-based authentication. Test scripts also check variable extraction, assertions, and error handling.
