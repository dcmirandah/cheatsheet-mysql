```
cd /var/www
chown -R www-data:www-data *
find . -type d -exec chmod 775 {} \;
find . -type f -exec chmod 664 {} \;
find / -name ".htaccess" -exec chmod 604 {} \;
find / -name ".htaccess" -exec chown www-data:www-data {} \;
```
