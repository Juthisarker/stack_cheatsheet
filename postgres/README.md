# Access PostgreSQL using the psql command-line tool
psql -U postgres

# List all databases
\l

# Alternatively, list all databases using SQL
SELECT datname FROM pg_database;

# Create new databases with UTF8 encoding
CREATE DATABASE database_name WITH ENCODING 'UTF8';


# Connect to a specific database
\c database_name

# Exit the PostgreSQL command-line tool
\q

# Delete a database
DROP DATABASE db_name;

# Import an SQL file into a PostgreSQL database
psql -h localhost -U postgres -d database_name -f /path/to/your/file.sql

# Example: Import an SQL file into the "database_name" database
psql -U postgres -h localhost -d "database_name" -f "database_name".sql
