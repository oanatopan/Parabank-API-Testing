# TC_09_GetCustomerId - Get Customer Accounts


### 🛠 Steps:
1. **Open Postman** and make sure that the `ParaBank_Test` workspace is active.
2. **In the 03.Account_Management** folder, select the **GetCustomerId** request.
3. 
4. **Press** the **Send** button.
5. **Confirm** the success of the test in the **Test Results** tab.

---

### 📋 Request Details:
**Method:** GET
**URL:** `{{baseURL}}/customers/{{customerId}}/accounts.
* **Variables used:**
    * `{{baseURL}}` —  `https://parabank.parasoft.com/parabank/services/bank`
    * `{{customerId}}` —  12212
* **Body:** None.

---

### ✅ Run Results (Validation):
* **Status Code:** `200 OK`.
* **Test Results:**
    * `PASS` - Status code is 200.
    * `PASS` - Accounts list returned (Checks if `jsonData` is an array).


### 📌 Dependency:**
This test is a necessary step for any operation involving account setup, as it generates a list of available IDs for transfers or bill payments.
