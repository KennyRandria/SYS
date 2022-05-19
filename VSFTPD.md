V S F T P D:


La Mise à jour : $ sudo apt update

L'installation :$ sudo apt install vsftpd

Verification si ça s'est bien passé :

$ whereis vsftpd

cela mène aux chemin vers l'installation de vsftpd


Lancement du serveur:

$ sudo systemctl start nginx

verification du serveur :

$ sudo systemctl status vsftpd


Connection aux sevreur vsftpd:

$ ftp "votre address ip"

Ensuite ça demande le mot de passe local et le nom d'utilisateur.


<a href = 'https://github.com/KennyRandria/SYS/'>RETOUR</a>
