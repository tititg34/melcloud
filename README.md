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

Béta V1

Ajout  pour la direction des volet Verticale et Horizontal
Ainsi que les information de retour

Bug connue le chiffre disparer dans la commande de volet 

Futur remplacer les button  Curseur  en liste 
