# PHP-install-ubuntu
php install ubuntu

command:
----------
    sudo apt-get update
    sudo apt-get install php7.2
    php -v
    
Bellow Command is After instalation Apache Server(If need):
-----------------------------------------------------------
    ls /etc/apache2/mods-available/php*
    ls /etc/apache2/mods-enabled/php*
    sudo a2enmod php7.2
    apachectl -t
    sudo service apache2 restart
    ls /etc/apache2/mods-enabled/php*

Refernces: https://www.liquidweb.com/kb/install-php-7-2-ubuntu-16-04/
