# Installing PHP in windows ##

## Download PHP for windows from below link #
```
https://windows.php.net/download#php-8.3

https://windows.php.net/downloads/releases/php-8.3.7-Win32-vs16-x64.zip
```

# Download Apache form below link #
```
https://www.apachelounge.com/download/

https://www.apachelounge.com/download/VS17/binaries/httpd-2.4.59-240404-win64-VS17.zip
```
# I have extraced Apache and PHP as below #

```
D:\BCA_PROJECT\PHP\httpd\Apache24
D:\BCA_PROJECT\PHP\php-8.3.7
```
## Change envoirment variable in windows and add below under PATH
```
D:\BCA_PROJECT\PHP\php-8.3.7
D:\BCA_PROJECT\PHP\httpd\Apache24\bin
```
# Configruration changes
## Change below line from D:\BCA_PROJECT\PHP\httpd\Apache24\conf\httpd.conf
```
Define SRVROOT "D:/BCA_PROJECT/PHP/httpd/Apache24"
```
## Add below lines at the end of D:\BCA_PROJECT\PHP\httpd\Apache24\conf\httpd.conf
```
AddHandler application/x-httpd-php .php
AddType application/x-httpd-php .php .html
LoadModule php_module "D:/BCA_PROJECT/PHP/php-8.3.7/php8apache2_4.dll"
PHPIniDir "D:/BCA_PROJECT/PHP/php-8.3.7"
DirectoryIndex index.php
```
# Install Apache using below command 
## Open CMD as Administrator and navigate to 
```
cd D:/BCA_PROJECT/PHP/httpd/Apache24/bin

```
## Enter below command to install service
```
httpd.exe -k install
```
# Star the services from services.msc Apache2.4
