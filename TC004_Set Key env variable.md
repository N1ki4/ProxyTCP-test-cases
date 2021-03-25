
### Test Case Title: ###

Set SSLKEYLOGFILE environmental variable					

---

**Test Case ID:** 004

**Priority:** Medium

**Will be Automated:** No

**Description:**

Set SSLKEYLOGFILE environmental variable to decrypt and analyse TLS traffic with Wireshark. 

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Set the environment variable named SSLKEYLOGFILE to a file name sslkelog.log | | 
|       2       | Set the same file name path in the Master-secret field in Wireshark. Go to Preferences > Protocols > TLS |  |  |
