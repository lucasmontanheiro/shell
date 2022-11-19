# Installing PHP

https://www.digitalocean.com/community/questions/why-can-t-i-upgrade-to-php-7-3

Upgrade to php7.3
```
sudo apt-get install software-properties-common
sudo add-apt-repository ppa:ondrej/php
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install -y php7.3
```

Check php version
```
php -v
```

Had to also run to enable PHP
```
sudo apt-get install php libapache2-mod-php
sudo a2enmod mpm_prefork && sudo a2enmod php7.0
sudo service apache2 restart
```

Had to also install MySQL
```
apt-get update
apt-get install php-mysql
apt-cache search mysql

```