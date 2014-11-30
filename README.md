Simple CRUD winform with SQL local database connection
==


This is my CRUD in winform for fmi project


Step by step tutorial: Creating database on your PC
----

Step 1: Open SQL Management Studio 
	Connect to a local server.
	Create a new database, name doesnt matter.
	Create a new table, name it "users".
	The table should be with columns names "id" with data type int
	"username" - nchar(10), "password" - nchar(10), "email" - nchar(20)
	Save!

Step 2: Now you have the DB. Open Visual Studio -> View -> Server Explorer, 
	find your newly created database and connect. Then right click to
	the database click "properties" and copy the path of "connection string".

Step 3: Now you copied the connection string of your database. On the project, 
	find Form1.cs and paste the connection string in
	"SqlConnection cn = new SqlConnection(@"[PUT IT HERE]");

 So you are done! Congratulations!!! I hope I was useful :)     // Copyright © Erhan™ 
