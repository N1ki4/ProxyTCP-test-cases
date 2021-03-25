
### Test Case Title: ###

 Connection fails when the proxy protocol selected is other than SOCKS5										

---

**Test Case ID:** 026

**Priority:** Low

**Will be automated:** Yes

**Description:**

Check that connections fails when the browser proxy is configured with the protocol other than SOCKS5

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :----------------- | :-------------- |
|       1       | Execute Test Case ID-001 with following configuration_data | configuration_data = {Scheme: (default), Protocol: HTTPS, Server: 35.217.25.199, Port: 1080} |  |
|       2       | In the URL field paste url and press enter | https://wiki.archlinux.org/ | Connection timeout, error appeared: ERR_TIMED_OUT |


