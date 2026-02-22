# TC18_GetAllTransactions - Global History Retrieval

### 🛠 Steps:
1. **Postman is opened** and the environment is active.
2. **Navigate** to the **05.Transactions_History&Filtering** folder.
3. **Select** the **GetAllTransactions** request.
4. **Press** the **Send** button.
5. **Verify** that the response contains the complete data structure in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `GET`
* **URL:** `{{baseURL}}/accounts/{{accountId}}/transactions`
* **Variables used:**
    * `{{baseURL}}` — The ParaBank API base endpoint.
    * `{{accountId}}` — The unique account identifier used to fetch the complete history.
* **Body:** None.

---

### ✅ Run Results:
* **Status Code:** `200 OK`.
* **Test Results:**
    * `PASS` - Status code is 200.

---

### 📌 Dependency:
Depends on the account created in **Module 02** and the financial activity (deposits/transfers) performed in **Module 04** to ensure the database has records to return.
