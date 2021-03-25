### Test Case Title: ###

Proxy supports TLS version 1.3

---

**Test Case ID:** 020

**Priority:** Medium 

**Will be Automated:** Yes

**Description:**

Verify proxy works correctly with TLS 1.3 version. Inspect every step of the TLS connection like handshakes and negotiation of the session. 
Make sure to use website which uses TLS version 1.3 as test data.

---

**Procedure:**

---

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 | |
|       2       | Open Wireshark on your internet interface and set filters | tcp.port == 1080 && tls |  |
|       3       | Start capturing packets in Wireshark |  |  |
|       4       | Open page | https://en.wikipedia.org/wiki/Internet_Protocol | Page is opened, content loaded successfully  |
|       5       | Stop capturing packets in Wireshark |  | Capture is filtered and not empty |
|       6       | Find successful tcp connection, right click on it and select "Follow" > "TCP Stream" |  | Capture is filtered  |
|       7       | Verify client sends hello |  | Packet with Info "Client Hello" exists.|
|       8       | Verify server sends hello back and changes cipher spec |  | Packet with Info "Server Hello, Change Cipher Spec" exists. |
|       9       | Verify client changed cipher spec and also sent  verification data |  | Packet with Info "Change Cipher Spec, Application Data" exists.  |
|       10      | Verify client sends encrypted data  |  | Packet with Info "Application Data" exists, data is encrypted.  |
|       11      | Verify server responses with encrypted data  |  | Packet with Info "Application Data" exists, data is encrypted.  |

___
