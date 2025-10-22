```dataview
TABLE 
  length(rows) as "Aparições"
FROM "1. Mental notes/Events"
WHERE people-involved
FLATTEN people-involved as person
GROUP BY person AS "Pessoa"
SORT length(rows) DESC
```