
### Test Case Title: ###

Web page with different ports

---

**Test Case ID:** 015

**Priority:** Medium

**Will be Automated:** Yes

**Description:**

Examine how web page works with explicitly specified ports

---

**Procedure:**

---

|     ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 | |    
|       2       | Open web page | @testurl | Page opens |
|       3       | Open web page with port 80 | @testurl:80 | "This site can’t provide a secure connection" heading is shown |
|       4       | Open web page with port 443 | @testurl:443 | Page opens |
|       5       | Open web page with port 20222 | @testurl:20222 | "This site can’t be reached" heading is shown |
|       6       | Open web page with port 65535 | @testurl:65535 | "This site can’t be reached" heading is shown |



**Test data:**

|      ID       | @testurl |
| :------------ |:--------------|
|       1       | https://tools.ietf.org | 
|       2       | https://about.gitlab.com  | 
|       3       | https://en.wikipedia.org | 
---
