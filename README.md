###################
OPEN BURPSUIT
###################

FIREFOX -> settings > proxy > 127.0.0.1:8080
goto: http://burp    download CA certificate
FIREFOX -> settings > certificates > Autority > import (select Certi & check all boxes and import)
Now try opening google.com





############################################
Download and setup bWAPP user in mysql
############################################

Download BWAPP zip.
Extract into /var/www/html ( #unzip bwapp.zip -b /var/www/html ).
Login to mysql ( mysql -u root -p ).
MariaDB [(none)]> use mysql
MariaDB [mysql]> create user 'bwappu'@'localhost' identified by 'bwapp';
MariaDB [mysql]> grant all privileges on bWAPP.* to 'bwappu'@'localhost' identified by 'bwapp';
Vi settings.php { $db_username = "bwappu"   $db_password = "bwapp" }
BROWSER :  http://127.0.0.1/bWAPP/install.php
CLICK LOGIN (bee;bug )

###########################################
burpsuit pro crack
###########################################

download crack sw and unzip it
java -noverify -jar ESEdition.jar 
dpkg -i openlogic-openjdk-jre-8u352-b08-linux-x64-deb.deb 
update-alternatives --config java   (select 8)
