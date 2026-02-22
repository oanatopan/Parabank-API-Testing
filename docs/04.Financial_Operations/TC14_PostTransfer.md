# TC14_PostTransfer - Funds Transfer


### 🛠 Steps:
1. **In the 04.Financial_Operations** folder, select the **PostTransfer** request.
2. **Navigate** to the **Params** tab and ensure `fromAccountId`, `toAccountId`, and `amount` are populated.
3. **Verify the generated URL:** `{{baseURL}}/transfer?fromAccountId={{accountId}}&toAccountId={{toAccountId}}&amount={{amount}}`.
4. **Press** the **Send** button.
5. **Confirm** the success of the test in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `POST`
* **Endpoint:** `{{baseURL}}/transfer`
* **Variables used:**
    * `{{accountId}}` — **Value:** 12345 | Source account (Debtor).
    * `{{toAccountId}}` — **Value:** 14454 | Destination account (Creditor).
    * `{{amount}}` — **Value:** 500 | The amount transferred between the accounts.
* **Body:** None.

---

### ✅ Run Results (Validation):
* **Status Code:** `200 OK`.
* **Response Time:** 412 ms.
* **Test Results:**
    * `PASS` - Transfer completed successfully.

---

### 📌Dependency:
Depends on **TC07/TC08** (for account creation) and **TC12** (to make sure the main account has enough money).
