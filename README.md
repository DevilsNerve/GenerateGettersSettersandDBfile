# README for PHP Database Class/DB Generator

This PHP script is a powerful tool designed to automate the creation of PHP classes and database (DB) classes for each table in a MySQL database. It establishes a PDO connection to a specified database and iterates over all tables. For each table, it generates two PHP class files: one representing the table's structure (with properties and getters/setters for each column) and another for database interactions specific to that table.

## How It Works

1. **Place the generateGnSnDB.php file within your models folder:** Place the generateGnSnDB.php file within your models folder.
2. **Database Connection:** First, the script connects to your MySQL database using PDO with the provided connection details.
3. **Table Analysis:** It retrieves the list of all tables in the database and iterates over them.
4. **Class Generation:** For each table, it generates a PHP class file containing properties, a constructor, and getters and setters for each column in the table.
5. **DB Class Generation:** Additionally, it generates a PHP DB class file intended for database interactions related to the specific table.
6. **File Storage:** Both generated class files are saved in a specified directory, ready to be included in your project for immediate use.
7. **Script Execution** Simply execute the generateGnSnDB.php from your server to initiate the process.

## Setup

1. Configure the database connection details (`$host`, `$db`, `$user`, `$pass`, `$charset`) at the beginning of the script.
2. Place the script in your project directory.
3. Run the script to generate the class files.
