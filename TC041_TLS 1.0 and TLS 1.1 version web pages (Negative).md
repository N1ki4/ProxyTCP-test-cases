### Test Case Title: ###

TLS 1.0 and TLS 1.1 version web pages (Negative)

---

**Test Case ID:** 041

**Priority:** Low 

**Will be Automated:** No

**Description:**

Verify Browser shows “Not Secure” warning when opening TLS 1.0 and TLS 1.1 version web pages. Browser may not load page and show "Your connection is not fully secure" or just show warning icon near url. TLS 1.0 and TLS 1.1 are deprecated. You can skip warning and visit the site, but your connection will be insecure and not encrypted. 

---

**Procedure:**

---

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 | |
|       2       | Open page | https://bestpeople.name | Browser throws "Privacy Error", heading "Your connection is not fully secure" is shown. Error "NET::ERR_SSL_OBSOLETE_VERSION" |
|       3       | Open page | https://receipt1.seiko-cybertime.jp | Browser throws "Privacy Error", heading "Your connection is not fully secure" is shown. Error "NET::ERR_SSL_OBSOLETE_VERSION"

---
