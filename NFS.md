N F S :

-D'abord la mis à jour des packages avec : apt-get install nfs-kernel-server 

mais il faut ajouter un dossier dans /var et droits absolu pour tous les root.
puis : mkdir /var/shared-data ;
chown root:root /var/shared-data;
chmod 755 /var/shared-data;

Partage de dossier :/etc/exports 

lecture seul et tous le monde peut y accéder :
 /var/a-public-folder *(ro,insecure,all_squash)
 
Après redémarrer le serveur NFS avec:
service nfs-kernel-server restart

Ensuite récupérer l'adresse IP serveur pour s'y connecter sur machine client : ip addr

Pour le côté client, on l'installe avec : apt-get install nfs-common
showmount -e 198.165.0.250 permet d'afficher du genre : Export for 198.165.0.250 : /home/nfs 198.165.10.10/24

On peut monter une machine serveur sur le client avec : mkdir/home/nfs
puis : mount -t nfs 198.165.0.250:/home/nfs /home/nfs
Pour vérifier le montage on tape : df -h 

<a href = 'https://github.com/KennyRandria/SYS/'>RETOUR</a>
