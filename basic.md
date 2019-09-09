Select 
```
/_api/web/lists/getbytitle('infolist')/items?$select=ID,Title,Employee,company
```

Order by
```
&$orderby= Employee asc
&$orderby= Employee desc
```

Filter
```
$filter=Employee eq ‘parth'
$filter=ID eq 2
$filter=Start_x0020_Date le datetime'2016-03-26T09:59:32Z'
$filter=( Modified le datetime'2016-03-26T09:59:32Z') and (ID eq 2)
$filter=startswith(Title,‘P’)
filter=month(Modified) eq 5
```

Numeric
- Lt
- Le
- Gt
- Ge
- Eq
- Ne

String
- startsWith
- substringof
- Eq
- Ne

Date and time
- day()
- month()
- year()
- hour()
- minute()
- second()

Paging
```
$top 5
$skip
```

Expand
```
$select=ID,Title,Employee,company,city/Id&$expand=city/Id
$select=Author/Title&$expand=Author/Id
```

Reference
----
https://www.c-sharpcorner.com/article/sharepoint-2013-using-rest-api-selecting-filtering-sortin/
