Unauthorized SQL injection vulnerability exists in Access OA

version:v2017 

Routing: general/hr/recruit/filter/delete PHP

The injected parameter $FILTER_ID exists

Here the code is very concise, when the $FILTER_ID is not empty, the parameter is concatenated directly into the SQL statement, which is bypassed because the parentheses are closed.

![WPS图片(1)](https://github.com/husterdjx/cve/assets/80690447/046bcecb-9e66-417d-87ae-bb1498ff3583)

POC

![WPS图片(2)](https://github.com/husterdjx/cve/assets/80690447/f93b5d08-3968-4f22-9d05-4dc3f42ddf90)
