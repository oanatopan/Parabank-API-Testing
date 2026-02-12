# TC05_PostShutdownJMSListener - Service Deactivation

### 🛠 Execution Steps:

1. **Preparation:** Ensure that the `ParaBank_Test` environment is active in Postman.
2. **Identification:** Navigate to the **01.System_Setup** folder and select the **PostShutdownJMSListener** request.
3. **Technical Inspection:**
    * Verify the HTTP Method is set to **POST**.
    * Confirm the URL is correctly mapped to `{{baseURL}}/shutdownJmsListener`.
4. **Execution:** Press the **Send** button.
5. **Result Audit:** Observe the Status Code and navigate to the **Test Results** tab to confirm the automated validation.

---

### 📋 Request Details:

* **Variables Used:** `{{baseURL}}` — **Value:** `https://parabank.parasoft.com/parabank/services/bank`
* **Logic Mechanism:** The request instructs the backend to stop the "listener" class responsible for the transaction queue, effectively halting asynchronous processing.
* **Body:** None (Empty).

---

### ✅ Run Results (Validation):

* **Status Code:** `200 OK` or `204 No Content` (Both codes are valid as they confirm the request was processed and the service state was changed).
* **Response Time:** ~385 ms
* **Test Results:**
    * `PASS` - The database has been cleaned (Note: In the ParaBank API, this is the standard success string for service state resets).

---

### 📌 Context & Dependency:

* **Role:** While this test marks the end of the system setup, it acts as a **Cleanup Check**.
* **Impact:** It demonstrates the ability to reset the service architecture to a "cold" state, ensuring the system can be restarted fresh for subsequent test iterations without residual thread conflicts.
