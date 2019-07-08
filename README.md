https://zmcdbp.com/easy-tutorial-using-verdaccio/

https://zmcdbp.com/fix-apache2-alias-vue-history-404/

http://www.10qianwan.com/articledetail/424394.html

LoadModule rewrite_module modules/mod_rewrite.so
<IfModule rewrite_module>
RewriteEngine On
# If an existing asset or directory is requested go to it as it is
RewriteCond %{DOCUMENT_ROOT}%{REQUEST_URI} -f [OR]
RewriteCond %{DOCUMENT_ROOT}%{REQUEST_URI} -d
RewriteRule ^ - [L]

# If the requested resource doesn't exist, use index.html
RewriteRule ^ /index.html
</IfModule>
