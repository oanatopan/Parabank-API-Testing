# TC03_PostStartupJMSListener - Primary Service Activation

### 🛠 Execution Steps:

1. **Context Preparation:** Open the Postman application and ensure that the `ParaBank_Test` environment is active.
2. **Resource Identification:** Navigate to the **01.System_Setup** folder in the collection and select the **PostStartupJMSListener** request.
3. **Configuration Inspection:**
    * Check the HTTP method: it should be set to **POST**.
    * Check the URL: it should use the correct environment variable in the form `{{baseURL}}/startupJmsListener`.
4. **Execution:** Press the blue **Send** button.
5. **Observation:** Observe if the status code returned in the Response section and verify that the response time is within acceptable limits for a system service.
6. **Result Validation:** Access the **Test Results** tab to confirm the execution of the automatic validation script.

---

### 📋 Request Details:

* **Variables used:** `{{baseURL}}` — `https://parabank.parasoft.com/parabank/services/bank`
* **Body:** None (Empty).

---

### ✅ Run Results:

* **Status Code:** `204 No Content` (Standard code confirming that the server has successfully processed the request, but does not need to return a message body).
* **Response Time:** ~150 ms 
* **Validation Script:** * `PASS` - Status code is 204
    * `PASS` - JMS Listener started successfully 

---

### 📌 Contextual Dependency:
This test is critical for the functioning of subsequent modules. If TC03 fails or is omitted, all money transfer tests in Module 04 will return false successes (the operation is created, but the money never "arrives" at its destination).
