This script implements a simple password manager using SQLite for storage and SHA-256 hashing for password creation. Here's a brief overview:

1) Authentication: The script asks for an admin password. If it matches the predefined password ("123456"), access is granted.

2) Database Connection: Connects to an SQLite database (pass_manager.db), and creates a table (KEYS) if it doesn't already exist.

3) Password Functions:
create_password(): Generates a password hash for a given service.
get_hex_key(): Creates a unique key for a service using the admin password and service name.
get_password(): Retrieves and generates the password for a given service.
add_password(): Adds a new service to the database and generates its password.
Main Loop: Provides options to:
Quit the program (q).
Store a new password (sp).
Retrieve an existing password (gp).
