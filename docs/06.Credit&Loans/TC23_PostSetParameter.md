# TC23_PostSetParameter - System Configuration

### 🛠 Steps:
1. **Open Postman** and navigate to the **06.Credit&Loans** folder.
2. **Verify** the `name` and `value` parameters in the **Params** tab to ensure they represent a valid system setting.
3. **Press** the **Send** button.
4. **Confirm** the successful update in the **Test Results** tab.

---

### 📋 Request Details:
* **Method:** `POST`
* **URL:** `{{baseURL}}/setParameter/{{name}}/{{value}}?name={{name}}&value={{value}}`
* **Variables used:**
    * `{{name}}` — loanProvider
    * `{{value}}` — jms
* **Body:** None.

---

### ✅ Run Results:
* **Status Code:** `204 No Content`.
* **Test Results:**
    * `PASS` — Status code is 204 (indicating successful processing).
   

---

### 📌 Dependency:
Setting the `loanProcessor` to a specific value before running **TC24_Post_Request_Loan** to ensure a predictable "Approved" or "Denied" outcome.
