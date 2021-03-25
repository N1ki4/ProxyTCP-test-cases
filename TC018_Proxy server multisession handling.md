
### Test Case Title: ###

 Proxy server multisession handling										

---

**Test Case ID:** 018

**Priority:** Medium

**Will be automated:** Yes

**Description:**

Check proxy ability to handle requests from multiple sessions simultaneously. Run test case with four different webpages, where each webpage represents different level of complexity in terms of number 
of requests and recourses.

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Execute precondition TC002 (proxy enabled) |  |  |
|       2       | Open 3 tabs in the browser | tab1: @testurl1 <br/>tab2: @testurl2 <br/>  tab3: @testurl3 | Pages loaded |
|       3       | Select all tabs and click reload |  | All pages reloaded successfully, no ERR_TIMED_OUT appeared |

---

**Test data:**

|      ID       | @testurl1 | @testurl2 | @testurl3 |
| :------------ |:--------------|:--------------|:--------------|
|       1       | https://wiki.archlinux.org/ | https://tools.ietf.org/html/rfc1928 | https://forums.wxwidgets.org/viewtopic.php?t=23247 |
|       2       | https://pypi.org/project/pyats/ |https://glossary.istqb.org/app/en/search/|https://www.gov.uk/foreign-travel-advice/somalia|
|       3       | https://github.com/rafi/awesome-vim-colorschemes |https://stackexchange.com/|https://www.facebook.com/|
|       4       | https://www.bookdepository.com/ <br/> publishers/Lulu-Com |https://stackoverflow.com/questions <br/> /9436534/ajax-tutorial-for-post-and-get|https://book-ye.com.ua/|

