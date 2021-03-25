
### Test Case Title: ###

Manual environment configuration 						

---

**Test Case ID:** 001

**Priority:** High

**Will be Automated:** No

**Description:**

Manual configuration of proxy server in Google Chrome browser with SwitchyOmega extension. Disable cache in developer tools 

---

**Procedure:**

___

|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Open "Google Chrome" browser in Incognito | | Browser is opened
|       2       | Click on "SwitchyOmega" extension |  | Popover is shown |
|       3       | Click "Options" |  | Settings window is opened |
|       4       | Fill "Proxy servers" table | @configuration_data | Table is filled with data  |
|       5       | Open Google Dev Tools  |  |  Dev Tools is shown |
|       6       | Select "Network" tab |  | Network tab is shown  |
|       7       | Select "Disable cache" checkbox |  | Checkbox is selected   |

**Test data:**  @configuration_data

|     Scheme       | Protocol |  Server  | Port |
| :------------ |:--------------| :---------- | :-------------- |
|     (default)     | SOCKS5 | 35.217.25.199 | 1080|
---