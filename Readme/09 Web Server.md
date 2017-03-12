### [Return to Readme](../README.md#webserver)
### Notes Web Server
================
##### Here are the list of web server to host web application

<a name="nginx"/>

* NginX command
	* sudo service nginx stop/start/restart
	* cd /etc/nginx 				(config file path)
	* cd /etc/nginx/sites-enabled 	(add new websites, delete the `default` file)
		* server {
		*     listen 81;
		*     server_name tom.quesbook.com;
		*     root /usr/share/nginx/html/Demo01/public;
		*     passenger_enabled on;
		*     # rails_env development;
		* }

<a name="passenger"/>

* Passenger
	* How to install passenger and nginx [link](https://www.phusionpassenger.com/library/install/nginx/install/oss/trusty/)
	* Config File Referenc [link](https://www.phusionpassenger.com/library/config/nginx/reference/#passenger_friendly_error_pages)

