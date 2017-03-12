### [Return to Readme](../README.md#database)
### Notes Database
================
##### Here are the database information


<a name="pgsql"/>
* Postgresql Install [link](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-14-04)

* Postgresql Command
	* After logon to the Ubuntu Server 
	* sudo su postgres
	* sudo /etc/init.d/postgresql status
	* sudo /etc/init.d/postgresql start
	* sudo /etc/init.d/postgresql stop	
	* sudo /etc/init.d/postgresql restart
	* sudo /etc/init.d/postgresql status
	* psql -U qbuser -d qbdemo01 -h 127.0.0.1 		(login with different user)
	* sudo chown -R postgres:postgres /etc/postgresql/9.3/main/		(PSQL config file for IP access)
	* drop database or user
		* dropuser -U postgres -e tomzhu
		* dropdb -U postgres -e tomzhudb
	* psql
		* \list (\l)
		* \connect (database_name)
		* \dt
		* CREATE DATABASE exampledb OWNER dbuser;
		* (list all users)
			* SELECT u.usename AS "User name",
			*   u.usesysid AS "User ID",
			*   CASE WHEN u.usesuper AND u.usecreatedb THEN CAST('superuser, create
			* database' AS pg_catalog.text)
			*        WHEN u.usesuper THEN CAST('superuser' AS pg_catalog.text)
			*        WHEN u.usecreatedb THEN CAST('create database' AS
			* pg_catalog.text)
			*        ELSE CAST('' AS pg_catalog.text)
			*   END AS "Attributes"
			* FROM pg_catalog.pg_user u
			* ORDER BY 1;
		* TRUNCATE TABLE table_name RESTART IDENTITY;

* Using Lunchy [link](https://www.moncefbelyamani.com/how-to-install-postgresql-on-a-mac-with-homebrew-and-lunchy/)
* Some Reference
	* JSONb for rails [link](https://antoine.finkelstein.fr/postgresql-jsonb-brings-nosql-into-rails)
	* PG vs Mysql [link](https://www.zhihu.com/question/20010554)
	* Ubuntu and PostgreSQL [link](http://www.mcbsys.com/blog/2014/05/connect-to-postgres-on-ec2-using-pgadmin/)
	* pg_hba.conf reload by pg_ctlcluster [link](http://dba.stackexchange.com/questions/72580/missing-the-pg-ctl-package-in-postgres-9-3-installation)
	* set password using \password [link](http://stackoverflow.com/questions/14564644/postgres-password-authentication-fails)
