1. Extract the .zip file to your web server, just put the "php_stock" folder under your "public_html".

2. Run "phpstockdb.sql" to generate the MySQL tables and populate some records

3. Change the database connection from "ewcfg12.php" file, find this code:

$EW_CONN["DB"] = array("conn" => NULL, "id" => "DB", "type" => "MYSQL", "host" => "localhost", "port" => 3306, "user" => "root", "pass" => "Elvis56", "db" => "php_stock", "qs" => "`", "qe" => "`");

and adjust this part: user" => "root", "pass" => "Elvis56", "db" => "php_stock"

with yours!

4. You need also to change the database connection info from the 2 following files:
- ewdbhelper12.php
- php_stockdb.php

find this code:

	// Database connection info
	var $Host = 'localhost';
	var $Port = 3306;
	var $Username = 'root';
	var $Password = 'Elvis56';
	var $DbName = 'php_stock';

and adjust it with yours!

5. For login, please use:

- Username: admin
- Password: master

cretit for  
Masino Sinaga