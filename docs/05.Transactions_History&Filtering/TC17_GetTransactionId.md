# TC17_GetTransactionId - Transaction Details

### 🛠 Steps:
1. **Postman** is opened and the environment is active.
2. **Navigate** to **05.Transactions_History&Filtering** and select **GetTransactionId**.
3. **Press** the **Send** button.
4. **Confirm** the validation of the received data in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `GET`
* **URL:** `{{baseURL}}/transactions/{{transactionId}}`
* **Variables used:**
    * `{{baseURL}}` — https://parabank.parasoft.com/parabank/api-docs/index.html - The ParaBank API base endpoint.
    * `{{transactionId}}` — The unique ID extracted from the transaction list 
* **Body:** None.

---

### ✅ Run Results:
* **Status Code:** `200 OK`
* **Test Results:**
    * `PASS` - Status code is 200.

---

### 📌 Dependency:
Depends on the `transactionId` 
