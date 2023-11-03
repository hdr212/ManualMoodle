# ManualMoodle

mkdir (example)


cd example


vagrant init ubuntu/jammy64


vagrant up --provider=virtualbox


vagrant ssh


sudo -s


apt update


apt upgrade


apt install -y php libapache2-mod-php


apt install -y php-fpm php-common php-mbstring php-xmlrpc php-soap php-gd php-xml php-intl php-mysql php-cli php-ldap php-zip php-curl


php -v


apt install -y apache2


apt install -y mysql-server


systemctl restart apache2


mysql


CREATE DATABASE bbdd;


CREATE USER 'usuario'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';


GRANT ALL ON bbdd.* to 'usuario'@'localhost';


exit


https://download.moodle.org/download.php/stable403/moodle-latest-403.zip


Mover el zip a la carpeta


mv /vagrant/moodle….zip /var/www/html/


cd /var/www/html/


ls


apt install unzip


unzip moodle….zip


ls


cd moodle


cp -R * ..


ls


cd ..


ll


ls


rm -r moodle


rm -r moodle….zip


rm -r index.html


cd /var/www/html


chmod -R 775 .


chown -R root:www-data .


exit


logout


vi Vagrantfile


config.vm.network "forwarded_port", guest: 80, host: 8080


config.vm.network "public_network"


vagrant reload


vagrant ssh


logout


vagrant reload


vagrant ssh


INICIAR SESION

cd /var/www/html

vi config.php

Cambias la IP


