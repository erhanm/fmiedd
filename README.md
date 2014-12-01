Simple CRUD winform with SQL local database connection
==


This is my CRUD in winform for fmi project


Step by step tutorial: Creating database on your PC
----

Step 1: Open SQL Management Studio 

	create database [yourDatabaseName]
	use yourDatabaseName
	
	create table roles
	(
	   roles_id int primary key not null,  //must be 1 for admin and 2 for members
	   role varchar(10) not null
	)
	create table users
	(
	id int not null,
	username varchar(10)
	password varchar(10)
	email varchar(20)
	role_id int foreign key references roles not null
	)
	Save!

Step 2: Now you have the DB. Open the project with Visual Studio -> View -> Server Explorer, 
	find your newly created database and connect. Then right click to
	the database click "properties" and copy the path of "connection string".

Step 3: Now you copied the connection string of your database. On the project, 
	find Form1.cs and paste the connection string in
	"SqlConnection cn = new SqlConnection(@"[PUT IT HERE]");

Step 4: And we are ready to open the application. When the application runs a login form will appear.
	Type username:admin, password:admin.	

 So you are done! Congratulations!!! I hope I was useful :)     // Copyright © Erhan™ 
