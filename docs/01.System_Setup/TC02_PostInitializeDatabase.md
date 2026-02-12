# TC02_PostInitializeDatabase - Environment Population


### 🛠 Steps:

1. **Verify** that the `ParaBank_Test` environment is active in Postman.
2. **Navigate** to the **01.System_Setup** folder and select the **PostInitializeDatabase** request.
3. **Inspect** the request to confirm the HTTP `POST` method and the `{{baseURL}}/initializeDB` endpoint.
4. **Press** the `Send` button to send the request to the server.
5. **Check** the response section to see if the status code is as expected and if the response time indicates that scripts are being processed correctly on the backend.
6. **Go** to the **Test Results** tab to validate the success of the automated test.

---

### 📋 Request Details:

* **Variables Used:** `{{baseURL}}` — `https://parabank.parasoft.com/parabank/services/bank` 
* **Data:** This action inserts the default user (Username: john / Password: demo) and generates active test accounts (e.g., 12345).
* **Body:** None (Empty).

---

### ✅ Run Results:

* **Status Code:** `204 No Content`
* **Response Time:** ~245 ms (average value based on test server performance).
* **Script Validation:** * `PASS` - The database has been initialized 

---

### 📌 Interdependence:
This test is directly conditioned on the success of TC01 (PostCleanDB). It must be run exclusively after resetting the database to ensure that the Master data is imported into a clean environment (State: Neutral), thus avoiding "Duplicate Entry" errors or corruption of incremental IDs.
