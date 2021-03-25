
### Test Case Title: ###

 Connection fails when the incorrect proxy server was selected										

---

**Test Case ID:** 027

**Priority:** Low

**Will be automated:** Yes

**Description:**

Check that connections fails when the browser proxy is configured with wrong proxy server IP address

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :----------------- | :-------------- |
|       1       | Execute Test Case ID-001 with following configuration_data | configuration_data = {Scheme: (default), Protocol: SOCKS5, Server: 10.0.0.1, Port: 1080} |  |
|       2       | In the URL field paste url and press enter | https://wiki.archlinux.org/ | Connection failed, error appeared: ERR_PROXY_CONNECTION_FAILED |


