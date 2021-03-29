
### Test Case Title: ###

 SOCKS5 protocol's handshake is implemented correctly									

---

**Test Case ID:** 022

**Priority:** High

**Will be automated:** Yes

**Description:**

Check the implementation of the SOCKS5 handshake and confirm it is compliant to the RFC 1928

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
|       6       | Find successful tcp connection, right click on it and select "Follow" > "TCP Stream" or Ctrl+Alt+Shift+T |  | Capture is filtered and have 4 Socks packets |
|       7       | Examine content of each Socks packet, make sure packets contain provided data |  |  |
|       7.1     | Packet 1, Dst: 35.217.25.199 |  | Accepted Auth Method: 0x0 (No authentication) |
|       7.2     | Packet 2, Src: 35.217.25.199 |  | Method[0]: 0 (No authentication) |
|       7.3     | Packet 3, Dst: 35.217.25.199 |  | Command: Connect (1) <br/> Remote name: wiki.archlinux.org <br/> Port: 443 |
|       7.4     | Packet 4, Src: 35.217.25.199 |  | Results(V5): Succeeded (0) <br/> Remote name: wiki.archlinux.org <br/> Port: 443 |



