
### Test Case Title: ###

Manual Firefox browser configuration 						

---

**Test Case ID:** 005

**Priority:** High

**Will be Automated:** No

**Description:**

Manual configuration of proxy server in Mozilla Firefox browser. Disable cache in developer tools 

---

**Procedure:**

___

|     ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Open "Mozilla Firefox" browser | | Browser is opened
|       2       | Click the menu button and select "New Private Window"|  | New window is opened |
|       3       | Click the menu button and select "Options" |  | Options window is opened |
|       4       | In the General panel, go to the "Network Settings" section, click "Settings..." | |  The "Connection Settings" dialog will open |
|       5       | Select "Manual proxy configuration" radiobutton |  |  |
|       6       | Fill "SOCKS Host" field, Click OK | @configuration_data |   |
|       7       | Open Firefox Developer Tools  |  |  Dev Tools is shown |
|       8       | Select "Network" tab |  | Network tab is shown  |
|       9       | Select "Disable cache" checkbox |  | Checkbox is selected   |

**Test data:**  @configuration_data

|  SOCKS Host  | Port |
| :---------- | :-------------- |
|   35.217.25.199       | 1080 |
---