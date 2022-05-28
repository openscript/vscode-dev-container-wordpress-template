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
1. Visit http://localhost:8080 in your browser