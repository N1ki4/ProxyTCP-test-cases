### Test Case Title: ###

TLS Certificate is not trusted (Negative)

---

**Test Case ID:** 040

**Priority:** Low

**Will be Automated:** No

**Description:**

Verify proxy does not change default browser behavior when requesting page with broken ssl certificate. Browser can show certificate authority invalid error or just show warning on the left to the url.

---

**Procedure:**

---

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 | |
|       2       | Open page | https://greenleadershiptrust.org | Browser throws "Privacy Error", heading "Your connection is not private" is shown. Error "NET::ERR_CERT_COMMON_NAME_INVALID" |
|       3       | Open page | https://www.grupoemsa.org | Browser throws "Privacy Error", heading "Your connection is not private" is shown. Error "NET::ERR_CERT_AUTHORITY_INVALID

---
