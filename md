## №1
```sql
SELECT p.id AS p_id, COUNT(pv.id) AS count_of_visits FROM person p
JOIN person_visits pv ON pv.person_id = p.id
GROUP BY 1
ORDER BY p_id ASC, count_of_visits DESC
```

