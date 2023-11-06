# Installation Guide

This Installation Guide is prepared for **Ubuntu** Operating System. Of course, you can use any unix-based system, but in this case you need to adopt this manual by youself.
Before your start make sure your have a **dedicated (virtual) server with root permission**. On a usual hosting the system will not work!

## 1. Linux Server Preparation
This section will describe how to prepare server for an installation of AtroCore Application.
* [Apache web server preparation](./web-server-preparation-apache.md) (RECOMMENDED)
* [Nginx web server preparation](./web-server-preparation-nginx.md)

## 2. Install AtroCore (AtroPIM, AtroDAM, etc) Application
This section describes how to install AtroCore Application on the prepared web server.

### 1. Create your project directory (if not exists yet)
> if the directory already exists, remove everything inside the directory.

To create the directory, run the command:
```
mkdir /var/www/my-atrocore-project 
```
> **my-atrocore-project** – project name

### 2. Go inside of your project directory
```
cd /var/www/my-atrocore-project 
```

### 3. Download project files

> Git may be used for this step, so make sure that [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) is installed. Please note, it is still possible to install the application without having `git` (see 3.6).

> It is essential, that you use the composer version, which is embedded in our software, because this version contains some of our modifications needed for backup and restoring of the system files and the database. That is why `php composer.phar update` is used. Please **DO NOT** use composer, which is installed on your server as it does not contain the required modifications.

#### 3.1. If you want to install AtroPIM and AtroDAM with demo data
> Demo data can be installed only for MySQL database system.

run
```
git clone https://github.com/atrocore/skeleton-pim.git . && php composer.phar self-update && php composer.phar update
```

#### 3.2. If want want to install the AtroPIM and AtroDAM without demo data

run
```
git clone https://github.com/atrocore/skeleton-pim-no-demo.git . && php composer.phar self-update && php composer.phar update
```

#### 3.3. If you want to install AtroDAM with demo data
> Demo data can be installed only for MySQL database system.

run
```
git clone https://github.com/atrocore/skeleton-dam.git . && php composer.phar self-update && php composer.phar update
```

#### 3.4. If you want to install AtroDAM without demo data

run
```
git clone https://github.com/atrocore/skeleton-dam-no-demo.git . && php composer.phar self-update && php composer.phar update
```

#### 3.5. If you want to install AtroCore only
Please install AtroDAM and than remove AtroDAM module via Administration > Module Manager.

#### 3.6. Installation without `git` 
If you have no git installed you may still copy the files to the project folder manually.

You can download the files from one of this directory:
- https://github.com/atrocore/skeleton-pim
- https://github.com/atrocore/skeleton-pim-no-demo
- https://github.com/atrocore/skeleton-dam 
- https://github.com/atrocore/skeleton-dam-no-demo

Than upload the files to your project folder and run
```
php composer.phar update
```

### 4. Change recursively the user and group ownership for your project files
```
chown -R www-data:www-data /var/www/my-atrocore-project/
```
> Ubuntu and Debian use **www-data** as a standard user for the webserver. This can also be one of the following: www, apache2, psacln etc.

### 5. Change the permissions for project files
```
find . -type d -exec chmod 755 {} + && find . -type f -exec chmod 644 {} +;
```
```
find client data custom upload -type d -exec chmod 775 {} + && find client data custom upload -type f -exec chmod 664 {} +
```    
### 6. Configure the crontab
   6.1. Open crontab for your webserver user, which is www-data in our case:
```
crontab -e -u www-data
``` 
   6.2. Add the following configuration:
```      
* * * * * /usr/bin/php /var/www/my-atrocore-project/index.php cron
```
> Please consider that `/usr/bin/php` is the correct path to PHP in our case. You may have other path. "cron" is the required parameter and should be definitely included for appropriate functioning.

### 7. Create MySQL database and user

User must have all privileges for the database, which should be used for the AtroCore Application. You can create database and user with all privileges by executing next few commands:

> If MySQL Database is not installed, you need to install it.

Connect to MySQL as a root user:
```
mysql -u root -p
```
Create the database **atrocore**:
```
CREATE DATABASE atrocore;
```
Create user **atrocore_user** with password **atrocore_password** and grant all needed privileges:
```
CREATE USER 'atrocore_user'@'localhost' IDENTIFIED BY 'atrocore_password';
GRANT ALL ON atrocore.* TO atrocore_user@localhost WITH GRANT OPTION;
```

### 8. Go to your Project URL to start the installation wizard 

Start the installation wizard for your AtroCore Application in the web interface from your URL: http://YOUR_PROJECT/ . Follow the instructions in the wizard.
