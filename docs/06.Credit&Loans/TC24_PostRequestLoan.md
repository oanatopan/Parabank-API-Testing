# TC24_Post_Request_Loan 

### 🛠 Steps:
1. **Postman is opened** and the workspace environment is active.
2. **Navigate** to the **06.Credit&Loans** folder and select **PostRequestLoan**.
3. **Press** the **Send** button.
4. **Confirm** the validation in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `POST`
* **URL:** `{{baseURL}}/requestLoan?customerId={{customerId}}&amount=5000&downPayment=500&fromAccountId={{accountId}}`
* **Variables used:**
    * `{{baseURL}}` — The ParaBank API base endpoint.
    * `{{customerId}}` — The unique identifier for the customer applying for the loan.
    * `{{accountId}}` — The source account for the down payment.
* **Body:** None.

---

### ✅ Run Results:
* **Status Code:** `200 OK`.
* **Test Results:**
    * `PASS` — Status code is 200 OK

---

### 📌 Dependency:
Depends on a valid `customerId` created during registration (Module 02) and an active `accountId` with sufficient funds for the down payment (Module 04). 
