
### Test Case Title: ###

 Heavy web page can be successfully reloaded multiple times										

---

**Test Case ID:** 037

**Priority:** Low

**Will be automated:** Yes

**Description:**

Reload web page multiple times with proxying enabled. The goal of this test case
is to check the sustainability of the proxy server. 

---

**Procedure:**

___


|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 |  |  |
|       2       | In the URL field paste url and press enter | https://stackoverflow.com/questions/9436534/ajax-tutorial-for-post-and-get  | Page loaded |
|       3       | From the "Network" tab of DevTools record failed requests R in case any occurred | R |  |
|       4       | Reload page |  | Page loaded |
|       5       | Repeat steps 3-4 five times and compare R |  | R0 = R1 = R2 = R3 = R4 |

---

