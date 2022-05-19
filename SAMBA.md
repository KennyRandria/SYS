S A M B A :

- Root connection(su)

-Mis à jour des packages avec : apt update

- Installez Samba avec la commande :apt-get install samba et il y a aussi : apt install samba

 <img src="https://github.com/KennyRandria/SYS/blob/main/images/samba-001-install-samba.png" alt="">

- Configurations :

 cd /home/

Création de fichier : mkdir smat

 sécurisation par changement de droit d'auteur avec : chmod 777 smat/

 Ajout d'un nouvel utilisateur,genre au hasard : useradd god

 Ajout de mot de passe (smbpasswd -a god) 

- On peut configurer maintenant avec nano: /etc/samba/smb.conf

-  Ajoutons le chemin [smat] - /home/smat valid users = dea browserable = yes writeable = yes

-Finalement, redémarer le serveur SAMBA Avec : /etc/init.d/samba restart

Et SAMBA devrait être installé et configuré

<a href = 'https://github.com/KennyRandria/SYS/'>RETOUR</a>
