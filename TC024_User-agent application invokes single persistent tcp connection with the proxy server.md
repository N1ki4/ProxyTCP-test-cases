
### Test Case Title: ###

 User-agent application invokes single persistent tcp connection with the proxy server									

---

**Test Case ID:** 024

**Priority:** High

**Will be automated:** Yes

**Description:**

Check that User-agent application invokes single persistent tcp connection with the proxy server during single session

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 |  |  |
|       2       | Open Wireshark on your internet interface and set filters | ip.addr == 35.217.25.199 |  |
|       3       | Start capturing packets in Wireshark |  |  |
|       4       | In the URL field paste url and press enter | https://wiki.archlinux.org/ | Page loaded |
|       5       | Stop capturing packets in Wireshark |  | Capture is filtered and not empty |
|       6       | Identify the number of established tcp connections by the number of 3 way handshakes |  | Only one tcp connection is established |




