
### Test Case Title: ###

 Website resources loading on first open of the super-light web page 									

---

**Test Case ID:** 012

**Priority:** High

**Will be automated:** Yes

**Description:**

Load webpage with proxying disabled and enabled and compare the number of failed requests for both cases. 
The goal of this test case is to verify that proxy server does not cause any data loss when page is loaded.

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-003 |  |  |
|       2       | In the URL field paste url and press enter | https://wiki.archlinux.org/ | Page loaded |
|       3       | From the "Network" tab of DevTools record the number of failed requests R0 | R0 |  |
|       4       | Execute precondition TC002 (proxy enabled) |  |  |
|       5       | In the URL field paste url and press enter | https://wiki.archlinux.org/ | Page loaded |
|       6       | From the "Network" tab of DevTools record the number of failed requests R1 and compare to R0 | R1 | R1 = R0 |

---

