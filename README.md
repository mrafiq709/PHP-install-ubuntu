# PHP-install-ubuntu
php install ubuntu

command:
----------
    sudo apt-get update
    sudo apt-get install php7.2
    php -v
    ls /etc/apache2/mods-available/php*
    ls /etc/apache2/mods-enabled/php*
    sudo a2enmod php7.2
    apachectl -t
    sudo service apache2 restart
    ls /etc/apache2/mods-enabled/php*
