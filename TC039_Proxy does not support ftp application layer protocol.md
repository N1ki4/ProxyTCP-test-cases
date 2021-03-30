
### Test Case Title: ###

 Proxy does not support ftp application layer protocol										

---

**Test Case ID:** 039

**Priority:** Low

**Will be automated:** No

**Description:**

Using curl terminal utility check if proxy server can handle ftp request. By design the ftp support is not provided.
For the testing purposes use VSFTP server on the remote VM (IP: 35.217.25.199, tcp.port: 21)

---

**Procedure:**


|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Open terminal window |  |  |
|       2       | With the proxy server running on the remote VM (IP: 35.217.25.199) execute curl command  | curl --socks5-hostname 35.217.25.199:1080 ftp://35.217.25.199 | No response within 10 seconds window |




