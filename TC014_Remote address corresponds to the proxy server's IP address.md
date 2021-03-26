
### Test Case Title: ###

Remote address corresponds to the proxy server's IP address					

---

**Test Case ID:** 014

**Priority:** High

**Will be Automated:** Yes

**Description:**

Verify web page remote address changes with proxy enabled

---

**Procedure:**

---

|     ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 | |     
|       2       | Open page | https://en.wikipedia.org/wiki/Internet_Protocol | Page is opened |
|       3       | Open Google Dev Tools (Network tab) |  | 'Main Page' Headers/General -  Remote Address: 35.217.25.199:1080 (Address and port of the proxy)  |

---
