
### Test Case Title: ###

 Proxy correctly transfers web page's http response status codes										

---

**Test Case ID:** 042

**Priority:** Medium

**Will be automated:** No

**Description:**

Using curl terminal utility check if proxy server transfers responses correctly. To test this feature use online service 
for generating http codes: https://httpstat.us.

---

**Procedure:**


|      ID       | Steps/Actions |  Test Data  | Expected Result |
| :------------ |:--------------| :---------- | :-------------- |
|       1       | Open terminal window |  |  |
|       2       | With the proxy server running on the remote VM (IP: 35.217.25.199) execute curl command  | curl --socks5-hostname 35.217.25.199:1080 -I https://httpstat.us/@code | Request was successful, first line in response is: "HTTP/2 @code"  |

---

**Test Data:**

|      ID       | @code | Description |
| :------------ |:------| :-----------|
|       1       | 200   | OK |
|       2       | 301   | Moved Permanently |
|       3       | 302   | Moved Temporary |
|       4       | 400   | Bad Request |
|       5       | 403   | Forbidden |
|       6       | 404   | Not Found |
|       7       | 500   | Internal Server Error |
|       8       | 502   | Bad Gateway |
|       9       | 503   | Service Unavailable |



