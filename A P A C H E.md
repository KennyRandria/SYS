#Apache

Installer et configurer le serveur Web Apache:

1 — Installation d’Apache
- Mis à jour des packages :
 sudo apt update
Installez le package apache2 :
  sudo apt install apache2

2 — Configurer le pare-feu :
- verifier les profils app d'ufw  :
 sudo ufw app list
* Autoriser le trafic sur le port 80 : sudo ufw allow 'Apache' puis vérifier avec : sudo ufw status

3 -Vérification du serveur Web
 Service :
 sudo systemctl status apache2

Normalement la Page d'acceuil par défaut d'apache est activée,
Pour y accéder ouvrez le navigateur en tapant : locahost:80 et voilà la page devrait se manifester

<a href = 'https://github.com/KennyRandria/SYS/'>RETOUR</a>
