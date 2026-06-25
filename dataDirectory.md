| Table       | Primary Key           | Description               |
| ----------- | --------------------- | ------------------------- |
| Orders      | order_id              | Stores order lifecycle    |
| Customers   | customer_id           | Customer location details |
| Order Items | order_id + product_id | Products purchased        |
| Payments    | order_id              | Payment information       |
| Reviews     | review_id             | Customer feedback         |
| Products    | product_id            | Product details           |
| Sellers     | seller_id             | Seller information        |


Relationship Diagram:

                Customers
                    │
                customer_id
                    │
                Orders
                    │
                order_id
                ┌───┼──────────────┐
                │   │              │
                │   │              │
                Items Payments Reviews
                │
                product_id
                │
                Products

                seller_id
                │
                Sellers