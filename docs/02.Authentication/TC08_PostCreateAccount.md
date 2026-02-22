# TC08_PostCreateAccount 

### 🛠 Steps:
1. **In the 02.Authentication** folder, select the **PostCreateAccount** request.
2. **Navigate** to the **Params** tab and write the following keys are present: `customerId`, `newAccountType`, and `fromAccountId`.
3. **Press** the **Send** button.
4. **Review** the **Test Results** tab to confirm validation.

---

### 📋 Request Details:
* **Method:** `POST`
* **URL:** `{{baseURL}}/createAccount?customerId={{customerId}}&newAccountType=1&fromAccountId={{fromAccountId}}`
* **Endpoint:** `{{baseURL}}/createAccount`
* **Variables used:**
    * `{{customerId}}` — The unique ID of the customer (retrieved from Login).
    * `{{fromAccountId}}` — The source account ID for initial funding.
* **Query Parameters:**
    * `customerId` (int)
    * `newAccountType` (0=CHECKING, 1=SAVINGS, 2=LOAN)
    * `fromAccountId` (int)
* **Body:** None.

---

### ✅ Run Results (Validation):
* **Status Code:** `200 OK`.
* **Test Results:**
    * `PASS` - Status code is 200.
    * `PASS` - Account type verification (Checks if the response matches CHECKING, SAVINGS, or LOAN).

### 📌 Dependency:
This test depends on the successful acquisition of the "customerId" from the authentication phase.
