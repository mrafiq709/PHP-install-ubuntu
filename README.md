# PHP-install-ubuntu
php install ubuntu
    
Install PHP 7.3:
---------------------
    sudo apt-get update
    sudo apt install php7.3
    
    sudo apt install php7.3-fpm php7.3-bcmath php7.3-cgi php7.3-cli php7.3-common php7.3-curl php7.3-dba php7.3-dev php7.3-json php7.3-mbstring php7.3-mysql php7.3-opcache php7.3-xml php7.3-xsl php7.3-zip libphp7.3-embed libapache2-mod-php7.3
    
   ##### List PHP Configuration File
    sudo vim /etc/php/7.<version>/apache2/php.ini
    sudo vim /etc/php/7.<version>/cli/php.ini
    sudo vim /etc/php/7.<version>/fpm/php.ini
    
   ##### Finding For PHP extension
    apt search php7.*
    
   ##### Switching PHP version
  - Interactive switching mode:
     ```sudo update-alternatives --config php```
  - Manual Switching:
     - Apache
     ```
     sudo a2dismod php5.6
     sudo a2enmod php7.3
     sudo service apache2 restart
     
     ```
        
     - Command Line:
     ```
     sudo update-alternatives --set php /usr/bin/php7.3
     ```

Bellow Command is After instalation Apache Server(If need):
-----------------------------------------------------------
    ls /etc/apache2/mods-available/php*
    ls /etc/apache2/mods-enabled/php*
    sudo a2enmod php7.2
    apachectl -t
    sudo service apache2 restart
    ls /etc/apache2/mods-enabled/php*

Refernces: https://www.liquidweb.com/kb/install-php-7-2-ubuntu-16-04/
