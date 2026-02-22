# TC06_GetLogin - User authentification

### 🛠 Steps:
1. **Open Postman** and make sure that the `ParaBank_Test` workspace is active.
2. **Navigate** to the **02.Authentification** folder and select the **GetLogin** request.
4. **Press** the **Send** button.
5. **Confirm** the success of the test in the **Test Results** tab.

---

### 📋 Request Details: 
**Method:** `GET` | **URL:** `{{baseURL}}/login/{{username}}/{{password}}`.
* **Variables used:** * `{{baseURL}}` — **Value:** `https://parabank.parasoft.com/parabank/services/bank`
    * `{{username}}` — **Value:** `john`
    * `{{password}}` — **Value:** `demo`
* **Body:** None (Parameters are passed in the Path).

---

### ✅ Run Results:
* **Status Code:** `200 OK`.
* **Test Results:** `PASS` - Status code is 200 (Success).
* **Dynamic Action:** ```javascript
var jsonData = pm.response.json();
pm.environment.set("customerId", jsonData.id);

---

### 📌 Dependency: 
* **Role:** Validates user credentials and initiates the session.
*  This test extracts the `customerId` from the response, which is essential for subsequent requests that require a specific user context (e.g., account details or transfers).
