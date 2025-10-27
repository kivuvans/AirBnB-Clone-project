# 🧩 Database Normalization – Airbnb Clone Project
# Objective

To ensure that the database design for the Airbnb Clone is optimized, free of redundancy, and adheres to the Third Normal Form (3NF).

# Understanding Normalization

Normalization is the process of organizing data in a database to:

Eliminate redundancy

Ensure data integrity

Simplify maintenance and updates

# Normalization Stages

# First Normal Form (1NF):

Each column holds atomic (indivisible) values.

Each record is unique.

# Second Normal Form (2NF):

Meets 1NF.

Every non-key attribute depends on the entire primary key (for composite keys).

# Third Normal Form (3NF):

Meets 2NF.

There are no transitive dependencies (non-key attributes depend only on the primary key).

# Normalization Steps Applied
# 1. User Table

Attributes:

user_id (PK), first_name, last_name, email, password_hash, phone_number, role, created_at



✅ 1NF: All attributes contain atomic values (no repeating groups).
✅ 2NF: The table has a single primary key (user_id), and all attributes depend on it.
✅ 3NF: No attribute depends on another non-key attribute — for example, email does not determine first_name.

✅ Result: The User table is in 3NF.
