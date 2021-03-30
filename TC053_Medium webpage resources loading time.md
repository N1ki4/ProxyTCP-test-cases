
### Test Case Title: ###

 Medium webpage resources loading time								

---
**Test Case ID:** 053

**Priority:** High

**Will be automated:** Yes

**Description:**

Load webpages with proxying disabled and enabled and compare loading time for both cases. Loading time for the case with proxy enabled should not exceed
the loading time without proxy for more than two times.

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute Test Case ID-003 (proxy disabled) |  |  |
|       2       | In the URL field paste url and press enter | https://github.com/rafi/awesome-vim-colorschemes | Page loaded |
|       3       | Fom DevTools record page loading time T0 | T0 |  |
|       4       | Execute Test Case ID-002 (proxy enabled) |  |  |
|       5       | In the URL field paste url and press enter | https://github.com/rafi/awesome-vim-colorschemes | Page loaded |
|       6       | Fom DevTools record page loading time T1 and compare it with T0 | T1 | T1 <= 2*T0 |

