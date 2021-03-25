
### Test Case Title: ###

 Connection fails when the proxy tcp port selected is other than 1080										

---

**Test Case ID:** 028

**Priority:** Low

**Will be automated:** Yes

**Description:**

Check that connections fails when the browser proxy is configured with wrong proxy server tcp port

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :----------------- | :-------------- |
|       1       | Execute Test Case ID-001 with following configuration_data | configuration_data = {Scheme: (default), Protocol: SOCKS5, Server: 35.217.25.199, Port: 8010} |  |
|       2       | In the URL field paste url and press enter | https://wiki.archlinux.org/ | Connection failed, error appeared: ERR_PROXY_CONNECTION_FAILED |


