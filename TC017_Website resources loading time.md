
### Test Case Title: ###

 Website resources loading time									

---
**Test Case ID:** 017

**Priority:** High

**Will be automated:** Yes

**Description:**

Load webpages with proxying disabled and enabled and compare loading time for both cases. Loading time for the case with proxy enabled should not exceed
the loading time without proxy for more than two times.
Run test case with four different webpages, where each webpage represents different level of complexity in terms of number of requests and recourses.
---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute precondition TC003 (proxy disabled) |  |  |
|       2       | In the URL field paste @testurl and press enter | @testurl | Page loaded |
|       3       | Fom DevTools record page loading time T0 | T0 |  |
|       4       | Execute precondition TC002 (proxy enabled) |  |  |
|       5       | In the URL field paste @testurl and press enter | @testurl | Page loaded |
|       6       | Fom DevTools record page loading time T1 and compare it with T0 | T1 | T1 <= 2*T0 |

---

**Test data:**

|      ID       | @testurl |
| :------------ |:--------------|
|       1       | https://wiki.archlinux.org/ |
|       2       | https://pypi.org/project/pyats/ |
|       3       | https://github.com/rafi/awesome-vim-colorschemes |
|       4       | https://www.bookdepository.com/publishers/Lulu-Com |

