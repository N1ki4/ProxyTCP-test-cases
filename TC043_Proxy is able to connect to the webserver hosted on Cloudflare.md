
### Test Case Title: ###

 Proxy is able to connect to the webserver hosted on Cloudflare									

---

**Test Case ID:** 043

**Priority:** High

**Will be automated:** Yes

**Description:**

Check if web resources hosted on Cloudflare are accessible through the proxy when using browser. Run test on 3 websites hosted on Cloudflare to make sure that proxy behavior is identical for all cases. 

---

**Procedure:**


|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 |  |  |
|       2       | In the URL field paste @testurl and press enter | @testurl | Page loaded |


---

**Test Data:**

|      ID       | @testurl |
| :------------ |:------|
|       1       | https://unpkg.com/   | 
|       2       | https://www.allaboutcookies.org/  | 
|       3       | https://forums.wxwidgets.org/   |




