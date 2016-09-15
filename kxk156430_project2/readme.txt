
1. DavisBase.java is the main file implementing the given specifications.
2. DavisBase.java class file calls the rest of classes that contain Select,Insert, Update,Drop table methods. 
3. Run the Executable jar using following run command in the ZIP file
4. Prompt (DavisSql) will be displayed.
5. Enter the commands.

Run command: 
java -jar Davisbase.jar

NOTE: 	All commands should end with a semicolon(;)
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Commands:
---------------------------------------------------------------------------------------------------------------------------------------------------------------------
1.SHOW TABLES			Displays all tables defined in the database.
2.CREATE TABLE 			Creates a new a new empty table.
3.INSERT INTO TABLE		Inserts a row/record into a table.
4.SELECT-FROM	 		style Query (Displays all rows of a table)
5.SELECT-FROM-WHERE 		style query (Displays Selected rows of the table depending on the WHERE Clause) Valid Operators in WHERE Clause: "=", ">", "<"
6.UPDATE TABLE-SET-WHERE	Update a record in the table		
7.DROP TABLE table_name		Drop the table from the database.
8.Help				Shows the help information.
9.EXIT 				Cleanly exits the program and saves all table in non-volatile files. 
---------------------------------------------------------------------------------------------------------------------------------------------------------------------
Test Queries Samples:
---------------------------------------------------------------------------------------------------------------------------------------------------------------------
1. Show tables;

2. CREATE TABLE Employee (
	row_id INT PRIMARY KEY,
	first_name TEXT NOT NULL,  
	last_name TEXT NOT NULL,  
	dep_level TINYINT,
	Salary_week SMALLINT,
	Annual_Salary BIGINT,
	work_hours REAL,  
	total_hours DOUBLE,
	birth_date DATE,
	join_date DATETIME
);

3. insert into Employee (row_id,first_name, last_name, dep_level, Salary_week, Annual_Salary, work_hours, total_hours, birth_date, join_date) values (1, 'Chris', 'Davis', 1, 900, 58600, 35.5, 40, '1996-05-11', '2016-03-23_13:52:23');

4. UPDATE Employee SET last_name='David' WHERE row_id = 1;

5. Select * from Employee;

6. Select * from Employee where row_id>1;

7. Select * from Employee where row_id<1;

8. Select * from Employee where row_id=1;

9. Drop table Employee;

10. help;

11. exit;




