### Задание 5 19.09.2023

№1
SELECT person.id, person.name, "age", "gender", "address", pizzeria.id, pizzeria.name, "rating" FROM "person", "pizzeria"
ORDER BY pizzeria.id ASC;

![image](https://github.com/Boloniez/bol/assets/145553853/fcc1fff0-f0d1-4a60-9b39-24fef1009895)

№2
SELECT "order_date" AS action_date, "name" FROM "person_order", "person"
WHERE "order_date" IN (SELECT "visit_date" FROM "person_visits") AND person_order.person_id = person.id
ORDER BY "order_date" ASC;

![image](https://github.com/Boloniez/bol/assets/145553853/a7402295-c046-4fd8-a7cb-817dcab0f4bb)



