pysqlcli
========

Python script to use as a sql client for Ora** DBs
--------------------------------------------------

- It needs the `cx_Oracle` library
- Right now it is compatible with `python 2.4` (Yes the server running this it a little bit old).

Examples
--------
- Connecting to the database  


        pysqlcli.py <user>/<password>@<db_host>:<db_port>/<database>
        
- Incommand help


        pysqlcli> \h
        \h:            Prints this help
        \d:            Lists all tables
        \d <table>:    Describes a table
        \c:            desactivates csv output
        \c <filename>: Activates csv output
        \q:            Exits the program
        <SQL command>: Executes SQL

- Autocomplete using `tab`


        pysqlcli> SELECT FROM TA
        TABLE_1        TABLE_2        ...        TABLE_N

- Listing all tables


        pysqlcli> \d
         TABLE_NAME                
        ----------------------------
         TABLE_1                
         TABLE_2    
         ...          
         TABLE_N
        (N rows)
