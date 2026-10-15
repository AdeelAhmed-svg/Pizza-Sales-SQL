# Pizza Sales Analysis with SQL

SQL analysis of a pizza sales dataset, answering 13 business questions. The full queries, results and visuals are in `Pizza Sales SQL Project.pdf`.

## Questions covered
- **Basic:** total orders, total revenue, highest-priced pizza, most common size, top 5 pizza types
- **Intermediate:** quantity by category, orders by hour, category distribution, average pizzas per day, top 3 pizzas by revenue
- **Advanced:** % revenue contribution per pizza type, cumulative revenue over time, top 3 pizzas by revenue per category

## Skills shown
SQL joins, aggregation, grouping, window functions, business-style analysis

Author: Adeel Ahmed | https://www.linkedin.com/in/adeelahmed-

## Insight

**Business question:** When should a pizza shop have the most staff and run promotions, and which menu items earn the most for each pizza sold?

**What I found (from my own query results):**
1. **Two rushes.** Orders peak between 12:00 and 14:00 (4,964 orders) and between 17:00 and 19:00 (4,775 orders). Together that is about 45.6% of all 21,350 orders in just four hours. Orders dip between 14:00 and 16:00 (about 1,500 per hour), and there are almost none before 11:00.
2. **Selling more pizzas does not always mean earning more.** Classic sold the most pizzas (14,888, about 30% of all pizzas) but earned 26.91% of revenue. Chicken sold the fewest (11,050, about 22%) but earned 23.96%, a bit more than Veggie (23.68%). The top 3 pizzas by revenue are all chicken pizzas: Thai ($43,434), Barbecue ($42,768) and California ($41,410).

**What I would suggest:** Plan extra staff for the lunch and evening rushes, test an offer in the 14:00 to 16:00 dip, and keep chicken pizzas visible on the menu.

**Caution:** This is one restaurant and about one year of data. It shows patterns, not causes. Percentages are my own calculation from the query results in the PDF.

## Notes and limitations
- My original SQL files were lost when I changed laptops. This PDF shows the queries and results exactly as I ran them.
- The orders-by-hour result is not sorted by hour.
- The "percentage contribution" query groups by category, not by individual pizza type.
- The top-5 slide shows the query without ORDER BY and LIMIT.
- The top-3-per-category result does not show the category column.
- "Most common size" counts order lines, not pizzas.
