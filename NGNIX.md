
N G N I X :

1. Comme d'habitude :
sudo apt-get update : mise à jour

sudo apt-get install nginx : installation

sudo systemctl start ngnix : pour activer /démarrer ngnix

Après, la vérification de l'installation avec : systemctl status ngnix :qui doit retourner active running
<img src="https://github.com/KennyRandria/SYS/blob/main/images/NGNIX2.png" alt="">

2. NGINX marche avec l'adresse Ip défini dans le naviguateur et devrait être bien installé

3. Configuration de NGINX se fait dans /etc/nginx dans le fichier de configuration nginx.conf

4. Exemple dans le dossier sites-enabled , on peut créer et modifier un site comme avec html css puis l'envoyer sur sites-available avec :

ln -s /etc/nginx/sites-available

5. Le redémarrage est absolument requis aprrès modification de ces fichiers comme nginx.conf,mime.types,sites-available, et executable avec :
sudo service nginx reload

sudo service nginx restart


Surtout bien vérifier la syntaxe de configuration avec :sudo nginx -t pour éviter les erreurs et après tout cela on peut redémarrer le service Nginx
le site devrait être accessible sur un lien http://nom attribué au site

<a href = 'https://github.com/KennyRandria/SYS/'>RETOUR</a>
