![Apache_logo](./images/Apache_logo.png)

# - Protéger l'accès à dossier ex : /var/www/html/

Créer un fichier caché nommé .htaccess dans /var/www/html.

touch /var/www/html/.htaccess

Saisir le code ci-dessous dans /var/www/html/.htaccess
```
AuthType Basic
AuthName "Zone protégée par mot de passe."
AuthUserFile /var/www/.htpasswd
Require valid-user
```
Créer un fichier caché nommé (.htpasswd) dans /var/www/.

Générer une clé de protection :

https://hostingcanada.org/htpasswd-generator/

