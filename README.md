# SulipySQLfuggveny

1. Feladat
A 'products' táblában határozd meg a 'standard_cost' mezőjének átlagértékét
a, az össezs rekord esetében,

  SELECT AVG(standard_cost) FROM products;
  
b, azon rekordok esetében, amelyeknél a 'list_price' 30-nál kisebb értékű,

  SELECT AVG(list_price) FROM products WHERE list_price < 30;
  
c, azon rekordok esetében, amelyeknél a 'category' mezőben 'Sauces' érték található!

   SELECT AVG(standard_cost) FROM products WHERE category = 'Sauces';
   
2. Feladat
A 'products' táblában határozd meg a 'standard_cost' mezőjének összértékét
a, az össezs rekord esetében,

  SELECT SUM(standard_cost) FROM products;
  
b, azon rekordok esetében, amelyeknél a 'list_price' értéke 20 és 50 közötti,

  SELECT SUM(list_price) FROM products WHERE list_price BETWEEN 20 AND 50;
  
c, azon rekordok esetében, amelyeknél a 'category' mezőben NEM 'Sauces' érték található!

  SELECT SUM(list_price) FROM products WHERE NOT category = 'sauces';

3. Feladat
A 'employees' táblában határozd meg azon alkalmazottak számát
a, akik Seattle-ben laknak,

  SELECT COUNT(id) FROM employees WHERE city = 'Seattle'
  
b, akiknek 'Sales Representative' munkakörben dolgoznak

  SELECT COUNT(id) FROM employees WHERE job_title = 'Sales Representative'
  
c, akiknek a keresztneve 'A' betűvel kezdődik!

  SELECT COUNT(id) FROM employees WHERE first_name LIKE 'A%';
  

  





















































