V S F T P D:


vsftpd est un serveur FTP sous licence GPL pour les systèmes UNIX, y compris Linux. Il est sécurisé et extrêmement rapide,C'est stable.

Bien qu'il soit petit pour des raisons de vitesse et de sécurité, de nombreuses configurations FTP plus compliquées sont réalisables avec vsftpd . En aucun cas une liste exclusive, vsftpd gérera :
   -Configurations IP virtuelles
   -Utilisateurs virtuels 
   -Fonctionnement autonome ou inetd
   -Puissante configurabilité par utilisateur
   -Limitation de la bande passante
   -Configurabilité IP par source
   -Limites IP par source
   -IPv6
   -Prise en charge du chiffrement via l'intégration SSL

.Installation et configuration :
La Mise à jour : $ sudo apt update

L'installation :$ sudo apt install vsftpd

<img src="https://github.com/KennyRandria/SYS/blob/main/images/VSFTPD.png" alt="">

Verification si ça s'est bien passé :

$ whereis vsftpd

cela mène aux chemin vers l'installation de vsftpd


Lancement du serveur:

$ sudo systemctl start nginx

verification du serveur :

$ sudo systemctl status vsftpd

<img src="https://github.com/KennyRandria/SYS/blob/main/images/VSFTPD2.png" alt="">

Connection aux sevreur vsftpd:

$ ftp "votre address ip"

Ensuite ça demande le mot de passe local et le nom d'utilisateur.


<a href = 'https://github.com/KennyRandria/SYS/'>RETOUR</a>
