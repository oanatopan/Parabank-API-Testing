# TC13_PostWithdraw - Fund Withdrawal

### 🛠 Steps:
1. **Open Postman** and make sure the environment is active.
2. **Navigate** to **04.Financial_Operations** and select **PostWithdraw**.
4. **Press** the **Send** button.
5. **Confirm** validation in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `POST`
* **URL:** `{{baseURL}}/withdraw?accountId={{accountId}}&amount={{amount}}`
* **Variables used:** * `{{baseURL}}` — API Base URL.
    * `{{accountId}}` — The source account ID.
    * `{{amount}}` — The amount to be deducted.
* **Body:** None.

---

### ✅ Run Results:
* **Status Code:** `200 OK`.
* **Response Time:** ~195 ms.
* **Test Results:** * `PASS` - Status code is 200.

---

### 📌 Dependency:
Depends on the balance created in **TC12_PostDeposit**
