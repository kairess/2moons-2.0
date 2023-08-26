```
brew tap shivammathur/php
brew install shivammathur/php/php@7.2
brew services start shivammathur/php/php@7.2

To enable PHP in Apache add the following to httpd.conf and restart Apache:
    LoadModule php7_module /usr/local/opt/php@7.2/lib/httpd/modules/libphp7.so

    <FilesMatch \.php$>
        SetHandler application/x-httpd-php
    </FilesMatch>

Finally, check DirectoryIndex includes index.php
    DirectoryIndex index.php index.html

The php.ini and php-fpm.ini file can be found in:
    /usr/local/etc/php/7.2/

brew install mariadb
mysql.server start
brew services start mariadb
sudo mysql -u root

brew install httpd
brew services start httpd

The default ports have been set in /usr/local/etc/httpd/httpd.conf to 8080 and in
/usr/local/etc/httpd/extra/httpd-ssl.conf to 8443 so that httpd can run without sudo.

Put files in /usr/local/var/www
```

## _v2.0.0	Danter14 17.02.2018_
[Modules] :
- Percentage with bar and text for real-time resources
- Number of players connect
- Planet change with arrows

[Bugs] :
- Fix of the language buddyList
- Fix bug for debris fields on the moon that replace the fields already in place by byazrail
- Fix bug, with destroyed moon by Kaizoku

[Improvements] :
- Ability to make high speed server

[Optimization] :
- Switching to php version 7.2

[Design] :
- Redesign of the bootstrap 4 login page
- Redesign Ingame by Danter14

[Panel administration] :
- none

## Developer
+ Project Leader
  - Danter14 (Hike)