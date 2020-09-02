1 .apt update
2. apt install apache2 apache2-utils curl mysql-server mysql-client php libapache2-mod-php php-mysql php-common php-mbstring php-xmlrpc php-soap php-gd php-xml php-mysql php-cli
3. wget https://files.phpmyadmin.net/phpMyAdmin/5.0.2/phpMyAdmin-5.0.2-all-languages.zip
4. sudo apt install unzip
5. unzip phpMyAdmin-5.0.2-all-languages.zip
6. mv phpMyAdmin-5.0.2-all-languages phpmyadmin









sudo apt update
sudo apt install apache2 apache2-utils curl mysql-server mysql-client php libapache2-mod-php php-mysql php-common php-mbstring php-xmlrpc php-soap php-gd php-xml php-mysql php-cli
check mysql and php version
1. mysql -v
2. php -v
Go to root folder
cd var/www/html
wget https://files.phpmyadmin.net/phpMyAdmin/5.0.2/phpMyAdmin-5.0.2-all-languages.zip
sudo apt install unzip
unzip phpMyAdmin-5.0.2-all-languages.zip
mv phpMyAdmin-5.0.2-all-languages phpmyadmin
Restart apache2 server
1. sudo service apache2 restart
Type sudo mysql
Create a new user
1.CREATE USER ‘username’@’localhost’ IDENTIFIED BY ‘password’;
CREATE DATABASE databasename;
GRANT ALL PRIVILEGES ON DATABASENAME.* TO ‘username’@’localhost’ WITH GRANT OPTION;
FLUSH PRIVILEGES;
Type Exit;
http://your_ip_address/phpmyadmin/index.php
Go to your root folder cd var/www/html
clone you project from github or bitbucket
add .env file and update database details in that file.
sudo apt install composer
Type Composer install
php artisan key:generate
copy index.php file from public folder and paste it into outside of the public folder.
Image for post
24. create one .htaccess file outside of the public folder
25. Go to /etc/apache2/apache2.conf
26. Change the line Allowoverride None into AllowOverride All
27. sudo a2enmod rewrite
28. sudo service apache2 restar
