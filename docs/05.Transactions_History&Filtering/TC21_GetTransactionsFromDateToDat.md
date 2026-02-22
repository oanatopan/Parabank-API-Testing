# TC21_GetTransactionsFromDateToDate 

### 🛠 Steps:
1. **Postman is opened** and the environment is active.
2. **Navigate** to the **05.Transactions_History&Filtering** folder and select **GetTransactionsFromDateToDate**.
3. **Verify** the `fromDate` and `toDate` parameters in the **Params** tab.
4. **Press** the **Send** button.
5. **Confirm** the validation results in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `GET`
* **URL:** `{{baseURL}}/accounts/{{accountId}}/transactions/fromDate/{{fromDate}}/toDate/{{toDate}}`
* **Variables used:** * `{{baseURL}}` — https://parabank.parasoft.com/parabank/services/bank
    * `{{accountId}}` — 12345 .
    * `{{fromDate}}` — 2026-02-21 The start date of the interval (format: `YYYY-MM-DD`).
    * `{{toDate}}` — 2026-02-21 The end date of the interval (format: `YYYY-MM-DD`).
* **Body:** None.

---

### ✅ Run Results:
* **Status Code:** `200 OK`.
* **Test Results:** * `PASS` — Status code is 200.

---

### 📌 Dependency:
Depends on financial transactions being previously recorded in the database during the selected timeframe ( in **Module 04**). 
