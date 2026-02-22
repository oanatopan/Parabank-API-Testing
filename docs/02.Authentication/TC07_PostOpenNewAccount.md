# TC07_PostOpenNewAccount - Create Account

### 🛠 Steps:
1. **Open Postman** and make sure that the `ParaBank_Test` workspace is active.
2. **Select** the **PostOpenNewAccount** request (Method: `POST`).
4. **Press** the **Send** button.
5. **Confirm** the success of the test in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** Post
* **URL** {{baseURL}}/createAccount?customerId={{customerId}}&newAccountType=0&fromAccountId={{accountId}}
* **Variables used:**
    * `{{customerId}}` — **Value:**  12212 | ID extracted from `GetLogin`.
    * `{{accountId}}` — **Value:** 12345 | Source account ID for initial funds.
* **Query Params:**
    * `newAccountType`: `0` (Constant for **CHECKING** type account).
* **Note:** Swagger documentation shows that types can be `CHECKING`, `SAVINGS`, or `LOAN`.

---

### ✅ Run Results (Validation):
* **Status Code:** `200 OK`.
* **Test Results:**
    * `PASS` - Account opened successfully.
    * `PASS` - Response contains account ID.

---

### 📌 Dependency:
 Executes the transition from identity validation to financial action (account creation).
 Critically depends on the success of **GetLogin**. Without a valid `customerId`, the server cannot associate the new account with an existing profile, resulting in a logic or authorization error.
