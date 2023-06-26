# Laravel
## Instalation:
* using sqlite: 
	- you should make sure that you have installed sqlite
		`sudo apt install sqlite3`
	- after that you should install the php extension
		`sudo apt install php-sqlite3`
	- change the .env file in this lines like this
		`DB_CONNECTION=sqlite`
		`DB_DATABASE=/home/williamjocoro/projects/laratest/database/database.sqlite` don't forget to create this file by doing `touch database/database.sqlite`
	- Run the migration
		`php artisan migrate`
	
## Blade
### Components

	
