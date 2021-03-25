
### Test Case Title: ###

 Website resources loading on reload with disabled cache										

---

**Test Case ID:** 013

**Priority:** High

**Will be automated:** Yes

**Description:**

Reload webpage multiple times with proxying enabled. The goal of this test case
is to check the sustainability of the proxy server. 
Run test case with four different webpages, where each webpage represents different level of complexity in terms of number 
of requests and recourses.

---

**Procedure:**

___


|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-002 |  |  |
|       2       | In the URL field paste @testurl and press enter | @testurl | Page loaded |
|       3       | From the "Network" tab of DevTools record the number of successful requests R | R |  |
|       4       | Reload page |  | Page loaded |
|       5       | Repeat steps 3-4 five times and compare the value of R |  | R0 = R1 = R2 = R3 = R4 |

---

**Test data:**

|      ID       | @testurl |
| :------------ |:--------------|
|       1       | https://wiki.archlinux.org/ |
|       2       | https://pypi.org/project/pyats/ |
|       3       | https://github.com/rafi/awesome-vim-colorschemes |
|       4       | https://www.bookdepository.com/publishers/Lulu-Com |

