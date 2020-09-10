# php72-centos7
https://tecadmin.net/install-php7-on-centos7/
yum install yum-utils -y
yum-config-manager --disable remi-php5*
yum-config-manager --disable remi-php74
yum-config-manager --disable remi-test
yum-config-manager --enable remi-php73
yum remove php php-*
yum install roundcube phpmyadmin -y
service httpd restart or service php-fpm restart
