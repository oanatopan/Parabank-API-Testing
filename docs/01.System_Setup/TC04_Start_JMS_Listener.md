# TC04_Start_JMS_Listener - Redundant Listener Check

### 🛠 Execution Steps:
1. **Ensure** that the previous test (TC03) has been successfully executed.
2. In the **01.System_Setup** folder, select the request named **Start JMS Listener**.
3. **Verify** that the method is **POST** and that the URL correctly targets the `{{baseURL}}/startupJmsListener` endpoint.
4. **Press** the **Send** button.
5. **Verify** that the server handles the redundant request without returning error codes in the 4xx or 5xx range.
6. **Check** the **Test Results** tab to confirm the validation script.

---

### 📋 Request Details:
* **Variables used:** `{{baseURL}}` — `https://parabank.parasoft.com/parabank/services/bank` 
* **Logic:** The test validates the stability of the API in the face of repetitive commands for managing system services.
* **Body:** None (Empty).

---

### ✅ Run Results:
* **Status Code:** `200 OK` or `204 No Content` (Both codes are acceptable, indicating that the desired service status is already active).
* **Response Time:** ~120 ms.
* **Script Validation:** * `PASS` - Status code is 200 or 204.

---

### 📌 Interdependence:
This test acts as a safety check.
