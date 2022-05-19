#Apache

°Apache est un logiciel de serveur web gratuit et open-source qui alimente environ 46% des sites web à travers le monde. Le nom officiel est Serveur Apache HTTP et il est maintenu et développé par Apache Software Foundation.°

Installer et configurer le serveur Web Apache:

1 — Installation d’Apache
- Mis à jour des packages :
 sudo apt update
Installez le package apache2 :
  sudo apt install apache2
  
  <img src="https://github.com/KennyRandria/SYS/blob/main/images/aPACHE2.png" alt="">

2 — Configurer le pare-feu :
- verifier les profils app d'ufw  :
 sudo ufw app list
* Autoriser le trafic sur le port 80 : sudo ufw allow 'Apache' puis vérifier avec : sudo ufw status

3 -Vérification du serveur Web
 Service :
 sudo systemctl status apache2

<img src="https://github.com/KennyRandria/SYS/blob/main/images/APACHE.png" alt="">

Normalement la Page d'acceuil par défaut d'apache est activée,
Pour y accéder ouvrez le navigateur en tapant : locahost:80 et voilà la page devrait se manifester

<a href = 'https://github.com/KennyRandria/SYS/'>RETOUR</a>
