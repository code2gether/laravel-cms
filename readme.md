# Laravel CMS

-   [System Requirements](#system-requirements)
-   [Installation](#installation)

## System Requirements

-   [PHP >= 7.1.3](https://nodejs.org/en/)
-   [Node.js](https://nodejs.org/en/)
-   [Composer](https://getcomposer.org/)
-   [MySQL](https://dev.mysql.com/doc/refman/8.0/en/windows-installation.html)
-   [Nginx](https://www.nginx.com/) or [Apache](https://httpd.apache.org/)
-   Enable PHP Extentions inside `php.ini` file
    -   OpenSSL PHP Extension
    -   PDO PHP Extension
    -   Mbstring PHP Extension
    -   Tokenizer PHP Extension
    -   XML PHP Extension
    -   Ctype PHP Extension
    -   JSON PHP Extension

### Installation

1. `git clone git@github.com:code2gether/laravel-cms.git`
2. `cd laravel-cms`
3.  Pull all required packages `composer install && composer update`
4.  Run `php artisan key:generate`
5.  Rename`.env-example` file  to `.evn`. 
6.  Create a new database in your Local phpMyAdmin with the correct credentials in `.env` file.
    ```DB_CONNECTION=mysql
     DB_HOST=127.0.0.1
     DB_PORT=3306
     DB_DATABASE=your-database-name
     DB_USERNAME=your database user name or root
     DB_PASSWORD=""
     ```
7.  Generate DB Tables `php artisan migrate`

#### Spin up PHP Dev Server

```
php artisan serve
```

#### Run Node Engine

If you change any JS or SCSS code then you need to run this command to see changes on time.

```
npm run watch
```

enjoy ;)
