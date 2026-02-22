# TC16_GetTransactionsAccountId - Account History

### 🛠 Steps:
1. **Open Postman** and chack if the workspace environment is active.
2. **Navigate** to the **05.Transactions_History&Filtering** folder and select **GetTransactionsAccountId**.
3. **Press** the **Send** button.
4. **Confirm** the validation in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `GET`
* **URL:** `{{baseURL}}/accounts/{{accountId}}/transactions`
* **Variables used:**
    * `{{baseURL}}` — The ParaBank API endpoint.
    * `{{accountId}}` — The unique account identifier extracted from previous modules.
* **Body:** None.

---

### ✅ Run Results (Validation):
* **Status Code:** `200 OK`.
* **Response Time:** ~312 ms.
* **Test Results:**
    * `PASS` - Status code is 200.
    * `PASS` - Verification: The `accountId` variable is present in the returned objects.

---

### 📌 Dependency:
Acts as the final verification layer for all financial activities performed in the suite.
Depends on the balance and activities created in **Module 04: Financial Operations** (e.g., **TC12_PostDeposit**, **TC14_PostTransfer**) to ensure there is transaction data to display in the history.
