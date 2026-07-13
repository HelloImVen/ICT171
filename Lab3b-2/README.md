## Progression for Lab3b-2

### Updating Ubuntu Packages.

I started by running `sudo apt update` on the Azure Ubuntu VM. I did this first so the package list was updated before installing the database software.

![Updating Ubuntu packages](./Screenshots/Screenshot%202026-07-12%20093933.png)

### Installing MariaDB.

I installed MariaDB server and client on the VM. MariaDB was the extra service I chose for this lab because it lets the server store and manage database information.

![Installing MariaDB](./Screenshots/Screenshot%202026-07-12%20094102.png)

### Starting and Enabling MariaDB.

After installing MariaDB, I started the service and enabled it so it could run automatically when the server starts.

![Starting and enabling MariaDB](./Screenshots/Screenshot%202026-07-12%20094313.png)

### Checking MariaDB Status.

I checked the MariaDB service status to make sure it was running properly. The output showed that MariaDB was active and ready to accept SQL requests.

![Checking MariaDB status](./Screenshots/Screenshot%202026-07-12%20094605.png)

### Opening the MariaDB Monitor.

I opened MariaDB from the terminal using `sudo mariadb`. This brought me into the MariaDB monitor where SQL commands could be typed.

![Opening MariaDB monitor](./Screenshots/Screenshot%202026-07-12%20094646.png)

### Viewing the Databases.

I used `SHOW DATABASES;` to list the available databases. This helped confirm that MariaDB was working and responding to SQL commands.

![Viewing databases](./Screenshots/Screenshot%202026-07-12%20094850.png)

### Creating the Server Services Table.

I selected the `ICT171_LAB` database and created a table called `server_services`. The table was made to store the service name and the purpose of the service.

![Creating server services table](./Screenshots/Screenshot%202026-07-12%20100255.png)

### Inserting Data into the Table.

I inserted a record into the `server_services` table for MariaDB. The purpose field described MariaDB as a database server for storing application data.

![Inserting data into table](./Screenshots/Screenshot%202026-07-12%20100524.png)

### Viewing the Table Data.

I used `SELECT * FROM server_services;` to display the table contents. The output showed the MariaDB record, which confirmed that the insert worked correctly.

![Viewing table data](./Screenshots/Screenshot%202026-07-12%20100703.png)

### My Conclusion

In this lab, I installed and tested MariaDB on my Azure Ubuntu server. I started by updating Ubuntu, then installed the MariaDB server and client packages. After that, I started and enabled the MariaDB service so it could run properly on the server.

Once MariaDB was running, I opened the MariaDB monitor and tested basic SQL commands. I checked the available databases, selected my `ICT171_LAB` database, created a table, inserted a record, and used a `SELECT` query to view the data.

This lab helped me understand how another server service can be installed and tested on a Linux cloud server. It also gave me more practice using database commands directly from the terminal.
