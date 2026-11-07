# Business data investigation: exercise rules

These fictional rules are the source of truth for this assignment. No industry research is required.

1. Use customers, orders, and refunds. IDs link refunds to orders and orders to customers; one order can have multiple refunds.
2. Gross sales for a period sum orders by order_date. Refunds for that period sum refunds by refund_date. Net sales equal gross sales minus refunds. Use UTC dates and half-open periods: start included, end excluded.
3. Use integer USD cents. Group order and refund totals separately before combining them; joining raw refund rows to orders can repeat order amounts.
4. Assign refunds to the segment of the customer on the original order. The records show amounts and dates, not why a customer requested a refund.
