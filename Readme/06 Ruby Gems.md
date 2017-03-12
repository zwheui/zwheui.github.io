### [Return to Readme](../README.md#rubygems)
### Notes Ruby Gems
================
##### Best Rails learning youtube [link](https://www.youtube.com/channel/UCSI77lJlzlCFPLdV1RSAoYQ)

<a name="rails"/>

* Rails
	* gem install rails --no-ri --no-rdoc 
	* rails new (Project name)
	* if we download a project we need to run `bundle install` first
	* 

* Rails @ variable [link](http://stackoverflow.com/questions/14319347/variables-in-ruby-on-rails)
	* title is a local variable. They only exists within it's scope (current block)
	* @title is an instance variable - and is available to all methods within the class.
	* In Ruby on Rails - declaring your variables in your controller as instance variables (@title) makes them available to your view.

* Rails Command
	* Generate Controller 	`rails g controller (controller name) (page name)`
	* Destory				`rails d controller (controller name)
	* Generate Model		`rails g model (model name) (model function name)`
	* Destory				`rails d model (model name)
	* rails g model QBEntity/EntValue --migration=false
	
* Rails Active Record ORM to DB
	* config/database.yml store the DB connection string
	* We can use the ENV variable to store the password so that the password is not show in the database.yml such as `password: <%= ENV['TOM_QBAPP_PASS'] %>`
	* We can also use local_evn.yml solution with [link](http://railsapps.github.io/rails-environment-variables.html)

* Rails Helpers (like HTML helper in C# MVC)
	* 

<a name="rake"/>

* rake
	* If meet 'You have already activated rake x.x.x, but your Gemfile requires rake y.y.y'
		* gem uninstall x.x.x
		* reference [link](http://stackoverflow.com/questions/6080040/you-have-already-activated-rake-0-9-0-but-your-gemfile-requires-rake-0-8-7)

	* rake db:create
	* rake db:schema:load
	* rake db:migrate:statue
	* rake RAILS_ENV=development

<a name="scss"/>

* SCSS/SASS
	* Difference [link](https://responsivedesign.is/articles/difference-between-sass-and-scss)

<a name="devise"/>

* Devise
	

<a name="railsapi"/>

* Rails API
	* gem install rails-api --skip-test-unit
	* 

* Rails get data from MS SQL and using storeprocedure 
	* [link](https://github.com/rails-sqlserver/activerecord-sqlserver-adapter/wiki/Using-TinyTDS)
	* [Github Link](https://github.com/rails-sqlserver/activerecord-sqlserver-adapter)
	* sudo gem install tiny_tds
  	* sudo gem install activerecord-sqlserver-adapter