# TC12_PostDeposit - Funds Deposit

### 🛠 Steps:
1. **Open Postman** and select the `ParaBank_Test` environment.
2. **Navigate** to the **04.Financial_Operations** folder.
3. **Select** the **PostDeposit** request.
4. **Press** the **Send** button.
5. **Confirm** the success of the test in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `POST`
* **Endpoint:** `{{baseURL}}/deposit`
* **Variables used:**
    * `{{baseURL}}` — **Value:** `https://parabank.parasoft.com/parabank/services/bank` 
    * `{{accountId}}` — **Value:** `12345` | The target account ID for the deposit.
    * `{{amount}}` — **Value:** `50000` | The amount of money added to the account.
* **Body:** None
---

### ✅ Run Results (Validation):
* **Status Code:** `200 OK`.
* **Test Results:**
    * `PASS` - This confirms the processing of the fund deposit.

---

### 📌 Dependency:
This operation is essential to provide sufficient funds for future withdrawal (**TC13**) or transfer (**TC14**) tests, preventing "Insufficient Funds" errors.
