
### Test Case Title: ###

 Proxy does not support http application layer protocol										

---

**Test Case ID:** 038

**Priority:** Low

**Will be automated:** No

**Description:**

Using curl terminal utility check if proxy server can handle http request. By design the http support is not provided

---

**Procedure:**


|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Open terminal window |  |  |
|       2       | With the proxy server running on the remote VM (IP: 35.217.25.199) execute curl command  | curl --socks5-hostname 35.217.25.199:1080 http://lutasprava.com | No response within 10 seconds window |




