# htaccess_react_cpanel

<IfModule mod_rewrite.c>
RewriteEngine On
RewriteBase /subdirectory
RewriteRule ^index\.html$ - [L]
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME} !-l
RewriteRule . /index.html [L]
</IfModule>
