Plugin melcloud pour jeedom  V4  

1- Aller dans la configuration du plugin :
Remplir votre login et mot de passe melcloud et cliquer sur le bouton obtenir token

2- Cliquer sur le bouton mettre a jour

3- Aller voir les pac détectés dans le plugin.
Rendre visible et activer les pacs.

le plugin est de floman321, je l'ai juste corrigé pour jeedom v4
la cose php7.3 qui génére un  Class 'object' not found 

la modif dans le fichier /var/www/html/plugins/melcloud/desktop/php/melcloud.php
à la ligne 97, remplacer
foreach (object::all() as $object) {
Par
foreach (jeeObject::all() as $object) {
