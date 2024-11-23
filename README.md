# vgsales_project_sql

## All-time Accumulated Sales by Genre
```
SELECT genre,
       ROUND(SUM(global_sales), 2) AS acc_sales
FROM vgsales
GROUP BY genre
ORDER BY acc_sales DESC;
```

## Genre Sales by Year 
```
SELECT genre,
       year,
       ROUND(SUM(global_sales), 2) AS acc_sales
FROM vgsales
GROUP BY year, genre
ORDER BY acc_sales DESC;
```
