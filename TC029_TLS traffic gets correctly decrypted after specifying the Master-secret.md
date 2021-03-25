
### Test Case Title: ###

 TLS traffic gets correctly decrypted after specifying the Master-secret										

---

**Test Case ID:** 029

**Priority:** High

**Will be automated:** Yes

**Description:**

Check that TLS traffic is being successfully decrypted after providing the Master-secret to TLS protocol
via SSLKEYLOGFILE system variable.

---

**Procedure:**


|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :----------------- | :-------------- |
|       1       | Execute Test Case ID-004 |  |  |
|       2       | Execute Test Case ID-002 |  |  |
|       3       | Open Wireshark on your internet interface and set filter | ip.addr == 35.217.25.199 |  |
|       4       | Start capturing packets in Wireshark |  |  |
|       5       | In the URL field paste url and press enter | https://wiki.archlinux.org/ | Page loaded |
|       6       | Stop capturing packets in Wireshark |  | Capture is filtered and not empty |
|       7       | In Wireshark find decrypted http2 traffic (green highlighted ) |  | Decrypted http2 traffic is present |


