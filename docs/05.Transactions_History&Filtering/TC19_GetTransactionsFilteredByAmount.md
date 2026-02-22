# TC19_GetTransactionsFilteredByAmount 

### 🛠 Steps:
1. **Postman is opened** and the environment is actived.
2. **Navigate** to **05.Transactions_History&Filtering** and select **GetTransactionsFilteredByAmount**.
3. **Press** the **Send** button.
4. **Confirm** in the **Test Results** tab that all returned records strictly match the requested amount.

---

### 📋 Request Details:
* **Method:** `GET`
* **URL:** `{{baseURL}}/accounts/{{accountId}}/transactions/amount/{{amount}}`
* **Variables used:**
    * `{{baseURL}}` — The ParaBank API base endpoint.
    * `{{accountId}}` — The unique identifier for the target account.
    * `{{amount}}` — The specific transaction value used as a filter (e.g., 500), consistent with operations in Module 04.
* **Body:** None.

---

### ✅ Run Results:
* **Status Code:** `200 OK`.
* **Test Results:**
    * `PASS` - Status code is 200.

---

### 📌 Dependency:
It depends on the specific amount successfully processed during previous operations, such as **TC12_PostDeposit** or **TC13_PostWithdraw** in **Module 04**. 
