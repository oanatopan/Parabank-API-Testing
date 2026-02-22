# TC22_GetTransactionsOnDate 


### 🛠 Steps:
1. **Postman is opened** and the workspace environment is active.
2. **Navigate** to the **05.Transactions_History&Filtering** folder and select **GetTransactionsOnDate**.
3. **Press** the **Send** button.
4. **Confirm** the results in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `GET`
* **URL:** `{{baseURL}}/accounts/{{accountId}}/transactions/onDate/{{date}}`
* **Variables used:** * `{{baseURL}}` — The ParaBank API base endpoint.
    * `{{accountId}}` — The unique account identifier being audited.
    * `{{date}}` — 22-02-2026

---

### ✅ Run Results:
* **Status Code:** `200 OK`.
* **Test Results:** * `PASS` — Status code is 200.
    * `PASS` — Date filtering functional

---

### 📌 Dependency:
Depends on the activity created on the specific date through previous operations, such as **TC12_PostDeposit** in **Module 04**. 
