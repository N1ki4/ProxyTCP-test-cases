
### Test Case Title: ###

 Proxy server's Payload Buffer does not affect integrity of  the tcp PDUs									

---

**Test Case ID:** 025

**Priority:** High

**Will be automated:** Yes

**Description:**

Check that Proxy server's Payload Buffer does not affect integrity of the tcp PDUs when merging segments of the tcp payload sent from the destination server.
To be able to run this test case manually run proxy server on your localhost through the WSL. Automation of this testcase requires a packet capturing facility implemented on the remote VM's internet interface.

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Open data.pcapng generated in TC023 in Wireshark in two windows |  |  |
|       2      | In the first window filter captured results to show only loopback data | tcp.stream == \<TSI1> | Capture is filtered and not empty |
|       3      | In the second window filter to show only external data | tcp.stream == \<TSI2> | Capture is filtered and not empty |
|       4      | In the second window find http2 request "GET /load.php?lang=en&modules=jquery&skin=vector&version=tqh7e" |  |  |





