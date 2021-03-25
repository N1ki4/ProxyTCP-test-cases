### Test Case Title: ###

Proxy supports TLS version 1.2 

---

**Test Case ID:** 019

**Priority:** Medium 

**Will be Automated:** Yes

**Description:**

Verify proxy works correctly with TLS 1.2 version. Inspect every step of the TLS connection like handshakes and negotiation of the session. 
Make sure to use website which uses TLS version 1.2 as test data.

---

**Procedure:**

---

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 | |
|       2       | Open Wireshark on your internet interface and set filters | tcp.port == 1080 && tls |  |
|       3       | Start capturing packets in Wireshark |  |  |
|       4       | Open page | https://tools.ietf.org/html/rfc5246 | Page is opened, content loaded successfully  |
|       5       | Stop capturing packets in Wireshark |  | Capture is filtered and not empty |
|       6       | Find successful tcp connection, right click on it and select "Follow" > "TCP Stream" |  | Capture is filtered  |
|       7       | Verify client sends hello |  | Packet with Info "Client Hello" exists.|
|       8       | Verify server sends hello |  | Packet with Info "Server Hello" exists. |
|       9       | Verify server provides a certificate, information for key exchange and indicated it has finished half of the handshake |  | Packet with Info "Certificate, Server Key Exchange, Server Hello Done" exists.  |
|       10      | Verify client provides information for key exchange, changed cipher spec and handshake was successful  |  | Packet with Info "Client Key Exchange, Change Cipher Spec, Encrypted Handshake Message" exists.  |
|       11      | Verify server created TLS session ticket key, changed cipher spec and handshake was successful  |  | Packet with Info "New Session Ticket, Change Cipher Spec, Encrypted Handshake Message" exists.  |
|       12      | Verify client sends encrypted data  |  | Packet with Info "Application Data" exists, data is encrypted.  |
|       13      | Verify server responses with encrypted data  |  | Packet with Info "Application Data, Application Data" exists, data is encrypted.  |

---
