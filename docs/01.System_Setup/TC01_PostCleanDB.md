# TC01_PostCleanDB - Database Reset


### 🛠 Steps:
1. **Open Postman** and make sure that the `ParaBank_Test` workspace is active.
2. **Navigate** to the **01.System_Setup** folder and select the **PostCleanDB** request.
3. **Check Method:** `POST` | **URL:** `{{baseURL}}/cleanDB`.
4. **Press** the **Send** button.
5. **Confirm** the success of the test in the **Test Results** tab.

---

### 📋 Request Details:
* **Variables used:** `{{baseURL}}` — **Value:** `https://parabank.parasoft.com/parabank/services/bank` 
* **Body:** None.

---

### ✅ Run Results:
* **Status Code:** `204 No Content`.
* **Response Time:** ~180 ms.
* **Test Results:** `PASS` - Status code is 204 (Success).

---

### 📌 Context :
* **Role:** Prepares the "neutral state" of the application.
* **Dependency:** This is the foundation test. It does not depend on other requests, but its success is critical for **TC02_PostInitializeDatabase**, as it prevents data conflicts (e.g., duplicate IDs) during database population.

### 📌 Context and Logical Interconnection:
* **Role:** Prepares the "neutral state" of the application.
