# Infotrixs
Task 1 commands
### 1. Install apache server on Ubuntu
`sudo apt install apache2`
### 2. Install php runtime and php mysql connector
`sudo apt install php libapache2-mod-php php-mysql`
### 3. Install MySQL server
`sudo apt install mysql-server`
### 4. Login to MySQL server
`sudo mysql -u root`
### 5. Change authentication plugin to mysql_native_password (Choose strong password)
`ALTER USER 'root'@localhost IDENTIFIED WITH mysql_native_password BY 'gayatri712';`
### 6. Create a new database user for wordpress
`CREATE USER 'gayatri'@localhost IDENTIFIED BY 'gayatri712'`;
### 7. Create a database for wordpress 
`create database wordpress`;
### 8. Grant all privileges on the database 'wordpress' to the newly created user
`GRANT ALL PRIVILEGES ON wordpress.* TO 'gayatri'@localhost
### 9. Download wordpress
`cd /tmp`
`wget`https://wordpress.org/latest.tar.gz
### 10. Unzip the file
`tar -xvf latest.tar.gz`
### 11. Move Wordpress folder to apache document root
`sudo mv wordpress/ /var/www/html`
### 12. Command to restart apache server
`sudo systemctl restart apache2`
OR
`sudo systemctl reload apache2`
