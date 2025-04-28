# Domino-s_Pizza  DAX Codes
Total Revenue = SUMX('Dominos', ('Dominos'[price]*'Dominos'[quantity]))  

Total Pizzas sold = sum(Dominos[quantity])

Total Number of orders = DISTINCTCOUNT(Dominos[order_id])

Average Pizza per Order = DIVIDE('Pizza Measures'[Total Pizzas sold],'Pizza Measures'[Total Number of orders])

Average Order Value = DIVIDE('Pizza Measures'[Total Revenue],'Pizza Measures'[Total Number of orders])
