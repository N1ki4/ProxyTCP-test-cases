
### Test Case Title: ###

 Website resources loading on first open										

---

**Test Case ID:** 012

**Priority:** High

**Will be automated:** Yes

**Description:**

Load webpage with proxying disabled and enabled and compare the number of successful requests for both cases. 
The goal of this test case is to verify that proxy server does not cause any data loss when page is loaded.
Run test case with four different webpages, where each webpage represents different level of complexity in terms of number 
of requests and recourses.

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-003 |  |  |
|       2       | In the URL field paste @testurl and press enter | @testurl | Page loaded |
|       3       | From the "Network" tab of DevTools record the number of successful requests R0 | R0 |  |
|       4       | Execute precondition TC002 (proxy enabled) |  |  |
|       5       | In the URL field paste @testurl and press enter | @testurl | Page loaded |
|       6       | From the "Network" tab of DevTools record the number of successful requests R1 and compare to R0 | R1 | R1 = R0 |

---

**Test data:**

|      ID       | @testurl |
| :------------ |:--------------|
|       1       | https://wiki.archlinux.org/ |
|       2       | https://pypi.org/project/pyats/ |
|       3       | https://github.com/rafi/awesome-vim-colorschemes |
|       4       | https://www.bookdepository.com/publishers/Lulu-Com |

