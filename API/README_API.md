# 🔌 API Testing – QA Full Project

This folder contains the **API Testing module** of the QA Full Project.  
Since the real SauceDemo platform does not provide public APIs, a **mock API simulation** has been created for demonstrating REST API testing and QA documentation skills.

This API project includes:
- REST API functional testing  
- Postman collection  
- Request/response validation  
- Test result screenshots  
- Error handling scenarios  
- API documentation (created manually for QA portfolio)

---

## 📁 Folder Structure
API/ ├── Postman_Collection.json ├── README_API.md └── TestResults/ ├── TestResult_1.png ├── TestResult_2.png └── TestResult_3.png

---

## 🌐 Base URL (Mock API)
All endpoints are simulated using a mock server for QA practice:

https://api.saucedemo.mock/server

This allows performing API testing even when the real system has **no backend endpoints**.

---

## 🔗 Endpoints Included

### **1) POST – User Login**

POST /auth/login

**Body:**
```json
{
  "username": "standard_user",
  "password": "secret_sauce"
}

Validations:

Status Code = 200

Response contains authentication token

Rejects invalid credentials (401)



---

2) GET – Inventory List

GET /inventory

Validations:

Status Code = 200

Response returns product list

Fields: id, name, price, image URL



---

3) GET – Single Item

GET /inventory/{id}

Validations:

Status Code = 200

Correct product details

Returns 404 for invalid ID



---

4) POST – Add to Cart

POST /cart/add

Body:

{
  "userId": 1,
  "productId": 4
}

Validations:

Status Code = 201

Confirmation message included

Cart count increases



---

5) GET – View Cart

GET /cart/{userId}

Validations:

Status Code = 200

Returned items match previous additions



---

🧪 Test Coverage

Feature	Status

Login API	✔ Tested
Inventory API	✔ Tested
Single Item API	✔ Tested
Add to Cart API	✔ Tested
Cart View API	✔ Tested
Error Handling	✔ Tested
Response Time Validation	✔ Tested



---

📊 Test Results

All screenshots of executed requests and responses are included in:

📁 API/TestResults/

Examples include:

Successful login

Failed login

Valid inventory fetch

Cart update

Error cases and negative tests



---

🎯 Purpose of This API Module

This section demonstrates:

Ability to design API tests when a real API does not exist

Understanding of REST structure (GET/POST)

Creating Postman documentation

Reporting defects based on API behavior

Building a professional QA Testing portfolio



---

👩‍💻 Author

Narges Soltani
QA Engineer (Manual, API, UI Automation)
GitHub: https://github.com/Narsis93
