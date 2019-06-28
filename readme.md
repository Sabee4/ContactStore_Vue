This project is to build a contact store or a contact manager application using Vue.js as front-end with sqlite as database.
-----------------------------------------------------------------------------------------------------
Contact Model Setup
-----------------------------------------------------------------------------------------------------
1. In the terminal, composer create-project laravel/laravel contactstore
2. In order to work with any of these assets and to compile them we have to first run NPM install
- Whenever we add anything in here in the assets and we need to recompile we can either run 
NPM run dev (which will just do it once and compile everything)
 or 
we can do NPM run watch (it will constantly watch those files and then compile every time we save)
3. We're going to use sqlite , which is a very very light file based database.
4.  create a new file, database.sqlite in database folder
5. Change in .env file	 
 	change app_name=Contact Store and DB connection=sqlite.
	And then just delete db_name,host,username,password from here because we don't need those.
	Save the file
6  config->database.php
	db_connection should be sqlite. Save the file 
7.  create a model called 
	In the terminal, php artisan make:model Contact -m
 8. In the migration file, add name, email and phone fields. Save the file
9. Run migration( php artisan migrate)
 
