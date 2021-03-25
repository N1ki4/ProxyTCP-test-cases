
### Test Case Title: ###

 Proxy server data transmission								

---

**Test Case ID:** 023

**Priority:** High

**Will be automated:** Yes

**Description:**

Check that proxy server transmits application data during the session of the client-server conversation correctly and without loses.
To be able to run this test case manually run proxy server on your localhost through the WSL. Automation of this testcase requires a
packet capturing facility implemented on the remote VM's internet interface.

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-001 with "Server" option set  to 127.0.0.1 |  |  |
|       2       | Execute Test Case ID-004 |  |  |
|       3       | Execute Test Case ID-002 |  |  |
|       4       | Open Wireshark on your internet and loopback interfaces and set filters | ip.addr == 135.181.27.174 or tcp.port == 1080 |  |
|       5       | Start capturing packets in Wireshark | |  |
|       6       | In the URL field paste url and press enter | https://wiki.archlinux.org/ | Page loaded |
|       7       | Stop capturing packets in Wireshark | | Capture is filtered and not empty |
|       8       | Identify loopback tcp stream and record it's stream index TSI1 | TSI1 |  |
|       9       | Identify external tcp stream and record it's stream index TSI2 | TSI2 |  |
|       10      | Save data to pcapng file | data.pcapng | |
|       11      | Filter captured results to show only loopback data | tcp.stream == \<TSI1> | Capture is filtered and not empty |
|       12      | In separate window open data.pcapng file and filter to show only external data | tcp.stream == \<TSI2> | Capture is filtered and not empty |
|       13      | Navigating between two windows compare http2 GET requests |  | Content of the corresponding request's headers and the total number of requests must be the same for both cases |
|       14     | Navigating between two windows compare http2 responses for the first two GET requests |  | Number and size of tcp PDU's sent in response must be the same for identical requests in both cases |



