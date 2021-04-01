### Bug Report Title: ###

Proxy wrong ports handling						

---

**Bug Report ID:** 004

**Severity:** High


**Description:**

Explicitly adding any port to the hostname redirects to the secure connection (port 443). Some hosts consider redirecting from not secure (80 port) to secure (443 port) connection default behaviour, some throws that "Site can`t provide a secure connection". 
Connecting to other ports than 80 and 433 should throw error, but current behavior is redirects every port to 443.  
---

**Steps to reproduce:**

___


|      ID       | Steps/Actions |  Expected Result | Actual Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 (enable proxy) |  |  |
|       2       | In the URL field paste https://wiki.archlinux.org:5000 and press enter | "This site can’t be reached" heading is shown. ERR_CONNECTION_TIMED_OUT | Page is opened successfully
|       3       | In the URL field paste https://wiki.archlinux.org:8000 and press enter | "This site can’t be reached" heading is shown. ERR_CONNECTION_TIMED_OUT | Page is opened successfully
|       4       | In the URL field paste https://wiki.archlinux.org:65535 and press enter | "This site can’t be reached" heading is shown. ERR_CONNECTION_TIMED_OUT | Page is opened successfully

---