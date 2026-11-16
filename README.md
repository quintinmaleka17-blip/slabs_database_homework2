1) The Dangers of Data Redundancy:
__________________________________

When a company stores a customer's physical address in three different tables instead of keeping it in a single
normalized Customers table. It can cause data redundancy and affect data integrity. When a customer changes their
address the company must update the address in all three tables. If one table is not updated the database will contain 
different addresses for the same customer. This could lead to confusion and incorrect deliveries. To avoid these problems
the company should store the customers address in one normalized customers table and use a primary key to reference that customer
in other tables.

2) Primary vs. Foreign Key Enforcement:
______________________________________

A Foreign Key constraint acts as a guardrail by ensuring that a record in one table can only reference a valid record in another table.
This prevents the creation of orphan records, which are records that reference data that does not exist.
