# TC25_BuyPosition - Stock Purchase Execution


### 🛠 Steps:
1. **Postman** is opened and the workspace environment is active.
2. **Navigate** to the **07.Investment_Portfolio** folder and select the **PostBuyPosition** request.
3. **Ensure the Path Variable** `customerId` is correctly populated with the value `12212`.
4. **Press** the **Send** button.
5. **Confirm** the validation in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `POST`
* **URL:** `{{baseURL}}/customers/:customerId/buyPosition?accountId={{accountId}}&name=Apple&symbol=AAPL&shares=10&pricePerShare=150`
* **Variables used:**
    * `{{baseURL}}` — https://parabank.parasoft.com/parabank/services/bank - The ParaBank API base endpoint.
    * `customerId`  — **Value:** `12212` 
    * `{{accountId}}` — **Value:** `12345` 
* **Body:** None.

---

### ✅ Run Results:
* **Status Code:** `200 OK`.
* **Test Results:**
    * `PASS` — Status code is 200 OK.

---

### 📌 Dependency:
Depends on the balance and account status established in **Module 03: Account Management**. 
