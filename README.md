# **MIT Admission**


## Installation
1. Clone the project `git clone https://github.com/sukanta7660/photography.git`

2. Go to project folder by entering `cd photography` command

3. Install composer following by this command: `composer install --ignore-platform-reqs`. Php must be the version of `7.2.5`

4. Copy `.env.example` file to `.env` on the root folder. You can type `copy .env.example .env` or `cp .env.example .env` using terminal in pathshala-api directory.

5. Open your database ***XAMPP / LAMP / HeidiSQL*** (Whatever you use).
   Create a new database with any database name. `For Example:  photography`
   Open your `.env` file and change the database name `DB_DATABASE` to whatever you have, username `DB_USERNAME` and password `DB_PASSWORD` field correspond to your configuration. By default, the username is `root` and you can leave the **password field empty**. *(This is for Xampp)*. By default, the username is `root` and password is also `root`. *(This is for Lamp)*.

6. Now run following commands on terminal:
```
php artisan key:generate
php artisan optimize:clear
```

7. You need to run following command for migrating the databases.

------------
>  **For Migrating Database:**
```
php artisan migrate
```

------------
>  **For Migrating Database (Fresh):**
```
php artisan migrate:fresh
```

------------

8. Then open browser and go to `http://localhost/photography`
