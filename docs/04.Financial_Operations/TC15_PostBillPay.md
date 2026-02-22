# TC15_PostBillPay - Bill Payment

### 🔍 Test Purpose:
To verify the system's ability to process bill payments to external payees from a specific user account.

---

### 🛠 Steps:
1. **In the 04.Financial_Operations** folder, select the **PostBillPay** request.
2. **Navigate** to the **Body** tab.
3. **Verify** the JSON structure contains payee variables (e.g., `{{name}}`, `{{street}}`).
4. **Check** the **Params** tab to ensure `accountId` and `amount` are set.
5. **Press** the **Send** button.
6. **Confirm** the success of the test in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `POST`
* **URL:** `{{baseURL}}/billpay?accountId={{accountId}}&amount={{amount}}`
* **Variables used:**
    * `{{baseURL}}` — **Value:** `https://parabank.parasoft.com/parabank/services/bank`
    * `{{accountId}}` — **Value:** `12345`
    * `{{amount}}` — **Value:** `500`
* **Body Variables (JSON):**
    * `{{name}}` — **Value:** `Oana Topan` | The name of the payment beneficiary.
    * `{{street}}` — **Value:** `Republicii` | The address of the bill beneficiary.


### ✅ Run Results (Validation):
* **Status Code:** 200 OK.
* **Response Time:** 180 ms.
* **Test Results:**
    * **PASS** - Bill payment processed.

---

### 📌 Dependency :
It is connected to GetLogin (Module 02) 
