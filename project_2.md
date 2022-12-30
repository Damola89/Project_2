I started by updating the server's package index using command `sudo apt update`

![apt update](./images%202/sudo_apt_update.png)

Nginx was installed on the server using `sudo apt install nginx`

![nginx installed](./images%202/nginx_installed_server.png)

I ran the command `sudo systemctl status nginx` to verify that nginx was successfully installed

![nginx test](./images%202/nginx_test.png)

I run `curl http://localhost:80` to check if i can locally access nginx on ubuntu

![nginx_ubuntu](./images%202/nginx_local_port.png)

I opened my browser to test if Nginx can respond to requests. 

![nginx_browser](./images%202/Nginx_browser_.png)

I installed Mysql using `sudo apt install mysql-server`

![install_mysql_server](./images%202/install_mysql_server.png)

I logged into mysql console using `sudo mysql`

![mysql_login](./images%202/sudo_mysql_login.png)

I set a password for the root user using mysql_native_password as default authentication method. After that, I exited mysql.

Started the interactive script by running `sudo mysql_secure_installation`

![mysql_interactive](./images%202/mysql_interactive_script_secure.png)

I tested to see if I am able to login into mysql console using `sudo mysql -p`

![mysql_login_test](./images%202/mysql_login_test.png)

Installed php, php-fpm and php-mysql using `sudo apt install php-fpm php-mysql`

![install_php-fpm_php_mysql](./images%202/install_php_fpm_php_mysql.png)

To use PHP processor on Nginx, i started by creating a directory structure on /var/www/html using `sudo mkdir /var/www/projectLEMP`

I thereafter assigned ownership of the directory using `sudo chown -R $USER:$USER /var/www/projectLEMP`

I then opened a new configuration file using `sudo nano /etc/nginx/sites-available/projectLEMP`

Added the bare-bones configuration to the blank file.

I activated the configuration by linking to the configuration file from nginx sites-enabled directory using `sudo ls -s /etc/nginx/sites-available/projectLEMP/etc/nginx/sites-enabled/`
Tested the configuration for syntax errors using `sudo nginx -t`

![nginx test](./images%202/nginx_conf_test.png)

I disabled default nginx host using `sudo unlink /etc/nginx/sites-enabled/default`

I reloaded nginx using `sudo systemctl reload nginx`

I thereafter created index.html file.

![nginx reload](./images%202/disable_nginx.png)

I tested the public IP using browser.

![public IP](./images%202/public_IP.png)