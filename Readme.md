## Installing PHP in windows ##

# Download PHP for windows from below link #
```
https://windows.php.net/download#php-8.3

https://windows.php.net/downloads/releases/php-8.3.7-Win32-vs16-x64.zip
```

# Download Apache form below ling
```
https://www.apachelounge.com/download/

https://www.apachelounge.com/download/VS17/binaries/httpd-2.4.59-240404-win64-VS17.zip
```
#
```
AddHandler application/x-httpd-php .php
AddType application/x-httpd-php .php .html
LoadModule php_module "D:/BCA_PROJECT/PHP/php-8.3.7/php8apache2_4.dll"
PHPIniDir "D:/BCA_PROJECT/PHP/php-8.3.7"
DirectoryIndex index.php
```
