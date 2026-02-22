# TC11_PostUpdateCustomer - Update Customer Information


### 🛠 Steps:
1. **Select** the **PostUpdateCustomer** request in Postman.
2. **In the Params tab**, verify the multiple variables being sent, such as `street`, `city`, `state`, `zipCode`, `phoneNumber`, `ssn`, `username`, and `password`.
3. **Press** the **Send** button.
4. **Confirm** the success of the test in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `POST`
* **Endpoint:** `{{baseURL}}/customers/update/{{customerId}}`
* **Query Params:** All customer profile fields (street, city, state, etc.) are passed as dynamic environment variables.
* **Variables used:** * `{{customerId}}` — The ID of the customer being updated.

---

### ✅ Run Results (Validation):
* **Status Code:** `200 OK`.
* **Test Results:** * `PASS` - Status code is 200.

---

### 📊 Execution Summary:
* **Average Response Time:** ~293 ms.
* **Errors:** 0.
* **Status:** 100% Success in validating account visualization and profile management.

---

### 📌 Dependency:
This test is essential for making sure that the system remains consistent even after administrative or personal profile changes.
