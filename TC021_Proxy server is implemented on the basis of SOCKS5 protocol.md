
### Test Case Title: ###

 Proxy server is implemented on the basis of SOCKS5 protocol										

---

**Test Case ID:** 021

**Priority:** High

**Will be automated:** Yes

**Description:**

Check the protocol type of the proxy server. Protocol must be Socks of version 5.

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 |  |  |
|       2       | Open Wireshark on your internet interface and set filters | ip.addr == 35.217.25.199 && socks |  |
|       3       | Start capturing packets in Wireshark |  |  |
|       4       | In the URL field paste url and press enter | https://wiki.archlinux.org/ | Page loaded |
|       5       | Stop capturing packets in Wireshark |  | Capture is filtered and not empty |
|       6       | Click on any packet and check Socks protocol version |  | Version: 5 |



