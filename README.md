# VSCode DevContainer Wordpress

Do you need a development, learning or teaching environment for a Wordpress project, which is quickly set up and contains all the tools you need? Maybe this is a good starting point.

You need [Visual Studio Code](https://code.visualstudio.com/) and the [Remote Containers](https://code.visualstudio.com/docs/remote/containers) extension.

## Features

- [x] PHP 8.1 with GD, zip and mbstring
- [x] MariaDB 10.4
- [x] PHPMyAdmin at port 8081
- [x] WP CLI

## First steps

1. Download Wordpress with `wp core download` (https://developer.wordpress.org/cli/commands/core/download/)
   - Add `--local=de_CH` or another prefered locale
   - Add `--version=6.0` or another prefered version
1. Start PHP server with `php -S localhost:8080`
1. Set up Wordpress
   - Via CLI
     1. Generate a config file with `wp config create --dbname=wordpress --dbuser=root --dbpass=mariadb --dbhost=db`
     1. Create database with `wp db create`
     1. Install Wordpress with `wp core install --url=localhost:8080 --title=Example --admin_user=example --admin_password=example123 --admin_email=example@example.com`
   - Via Browser
     1. Open PHPMyAdmin at http://localhost:8081 in your browser
     1. Create a database `wordpress` with `utf8_general_ci` as charset
     1. Visit http://localhost:8080 in your browser
     1. Fill out the form with database `wordpress`, database user `root`, database password `mariadb` and database host `db`.
     1. Fill out the site information as you like
