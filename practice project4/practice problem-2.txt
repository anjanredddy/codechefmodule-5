SELECT cuisine, 
COUNT(CASE WHEN category = 'Veg' THEN 1 ELSE NULL END)
FROM Orders
GROUP BY cuisine;