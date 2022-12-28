Installing the Nginx Web Server

I started by updating my server's package index using `sudo apt update` 

![update apt](./images%202/Update_server_index.png)

Proceeded to install Nginx using `sudo apt install nginx`

![Nginx install](./images%202/install_nginx.png)

To verify that nginx was succeefully installed. I seached using `sudo systemctl status nginx`

![Nginx status](./images%202/server_status.png)

to access the Nginx server on ubuntu, i used `curl http://localhost:80`

![Nginx_Ubuntu](./images%202/nginx_ubuntu.png)

Tested Nginx on browser by using `http://44.211.80.194`

![Nginx_browser](./images%202/nginx_browser.png)

Install mysql DBMS for starage using `sudo apt install mysql-server`

![mysql_install](./images%202/mysql_install.png)

log into mysql `sudo mysql`

![mysql_login](./images%202/mysql_login.png)

Defined user's password and started interactive script using `sudo mysql_secure_installation`

![mysql_installation](./images%202/mysql_interactive_script.png)

logged into mysql console using `sudo mysql -p`

![mysql_login](./images%202/mysql%20console_login.png)

Php-fpm and php-mysql were installed on the nginx server using `sudo apt install php-fpm php-mysql`

![php_fpm php_mysql](./images%202/php_fpm%20php_mysql.png)

I updated the server by using command `sudo apt update`

![server update](./images%202/server_update.png)

I installed nginx using `sudo apt install nginx`

![nginx install](./images%202/nginx_installed.png)

I verified to know if nginx was successfully installed using `sudo systemctl status nginx`

![nginx_ubuntu](./images%202/nginx_ubuntu.png)

I also tested nginx locally on ubuntu using `curl http://localhost:80`

![nginx_ubuntu](./images%202/nginx_test_ubuntu.png)