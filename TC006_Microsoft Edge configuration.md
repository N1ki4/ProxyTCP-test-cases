
### Test Case Title: ###

Manual Microsoft Edge browser configuration 						

---

**Test Case ID:** 006

**Priority:** High

**Will be Automated:** No

**Description:**

Manual configuration of proxy server in Microsoft Edge browser. Disable cache in developer tools 

---

**Procedure:**

___


|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Open "Microsoft Edge" browser | | Browser is opened |
|       2       | Get "SwitchyOmega" extension from "Edge Add-ons"|  |  |
|       3       | Click the menu button and select "New InPrivate window"|  | New private window is opened |
|       4       | Click on "SwitchyOmega" extension |  | Popover is shown |
|       5       | Click "Options" |  | Settings window is opened |
|       6       | Fill "Proxy servers" table | @configuration_data | Table is filled with data  |
|       7       | Open Microsoft Edge Developer Tools  |  |  Dev Tools is shown |
|       8       | Select "Network" tab |  | Network tab is shown  |
|       9       | Select "Disable cache" checkbox |  | Checkbox is selected   |
|       10      | Click on "SwitchyOmega" extension |  | Popover is shown |
|       11      | Select "proxy" option |  |  Circle became light blue |

**Test data:**  @configuration_data

|     Scheme       | Protocol |  Server  | Port |
| :------------ |:--------------| :---------- | :-------------- |
|     (default)     | SOCKS5 | 35.217.25.199 | 1080|
---