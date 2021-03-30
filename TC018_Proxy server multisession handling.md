
### Test Case Title: ###

 Multiple tabs simultaneous loading										

---

**Test Case ID:** 018

**Priority:** Medium

**Will be automated:** Yes

**Description:**

Check proxy ability to handle requests from multiple browser tabs simultaneously.

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 (proxy enabled) |  |  |
|       2       | Open 3 tabs in the browser | tab1: https://wiki.archlinux.org/ <br/>tab2: https://tools.ietf.org/html/rfc1928 <br/>  tab3: https://dev.mysql.com/doc/refman/8.0/en/ | Pages loaded |
|       3       | Select all tabs and click reload |  | All pages reloaded successfully, no ERR_TIMED_OUT appeared |
