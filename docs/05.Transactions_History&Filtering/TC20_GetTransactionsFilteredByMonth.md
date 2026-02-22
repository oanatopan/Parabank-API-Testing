# TC20_GetTransactionsFilteredByMonth - Monthly Filtering

### 🛠 Steps:
1. **Postman is opened** and `ParaBank_Test` environment is active.
2. **Navigate** to the **05.Transactions_History&Filtering** folder.
3. **Select** the **GetTransactionsFilteredByMonth** request.
4. **Verify the Params:** Ensure the `month` key is set (e.g., "All" ).
5. **Press** the **Send** button.
6. **Confirm** the results in the **Post-response** scripts tab.

---

### 📋 Request Details:
* **Method:** `GET`
* **URL:** `{{baseURL}}/accounts/{{accountId}}/transactions/month/{{month}}/type/{{type}}`
* **Variables used:**
    * `{{baseURL}}` — https://parabank.parasoft.com/parabank/api-docs/index.html -The ParaBank API base endpoint.
    * `{{accountId}}` — The unique account identifier.
    * `{{month}}` — Value: `All` | Defines the temporal filter.
    * `{{type}}` — Value: `Credit` | Defines the transaction category.

---

### ✅ Run Results:
* **Status Code:** `200 OK`.
* **Test Results:**
    * `PASS` — Status code is 200 OK.

---

### 📌 Dependency:
Depends on the transaction history populated in **Module 04**. 
