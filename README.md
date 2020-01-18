Plugin melcloud pour jeedom V4

1- Aller dans la configuration du plugin :
Remplir votre login et mot de passe melcloud et cliquer sur le bouton obtenir token

2- Cliquer sur le bouton mettre a jour

3- Aller voir les pac détectés dans le plugin.
Rendre visible et activer les pacs.

Le plugin est de Floman321, je l'ai juste corrigé pour jeedom V4


La cose php7.3 qui génére « Class ‘object’ not found »

La modif dans le fichier /var/www/html/plugins/melcloud/desktop/php/melcloud.php

la ligne 97, remplacer

foreach (object::all() as $object)

par

foreach (jeeObject::all() as $object)
