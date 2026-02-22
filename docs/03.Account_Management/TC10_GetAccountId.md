# TC10_GetAccountId - Specific account detail


### 🛠 Steps:
1. **Select** the **GetAccountId** request in Postman.
3. **Press** the **Send** button.
4. **Confirm** the success of the test in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** Get
* **URL:** `{{baseURL}}/accounts/{{accountId}}`
* **Variables used:**
    * `{{accountId}}` — **Value:** Target account ID (e.g., 12345).
* **Body:** None.

---

### ✅ Run Results (Validation):
* **Status Code:** `200 OK`.
* **Test Results:**
    * `PASS` - Status code is 200.
    * `PASS` - Verify account details (Confirms `jsonData` has property 'id').

---

### 📌 Dependency:** 
* Requires a valid `accountId`, typically obtained from **TC09_GetCustomerId** or the account creation steps (**TC07**/**TC08**). It is essential for checking balances before performing transactions.
