# Linux administration

## Pront
```
drwx-x-xw-x
c = caractère antaine
b = bloc usb
d = directory
l = lien symbolic
- = file
```

# arboressance

/bin = binaire
/sbin = binaire avec droit de root
boot = boot
dev = divice (disque / usb ... )
efi = boot
etc = editabale textural configration file ( fichier lier a la conf et au service )
home = user directory
lib = librairie system
mnt = mont pour monter les disque 
opt = optionnelle 
proc = information lier au proc
root = home de root
run = service en cour
srv = relative au serveur
sys = fichier system
tmp = temporaire
usr = fichier relatif au utilisateur et au logiciel installer sur le system
var = variable (tmp persistant)

# Lien sybolique et phisique

lien phisique avec les INODE

ls -i = inode 

le lien phisique renvoi au meme endroit que le fichier orginal alors que le lien symbolique créé un nouveau inode 


si on créé un lien phisique il renvois directement sur la donner
                    symbolique qui renvoi sur le fichier et non la dossier


ln file 1 file 3 #lien phisique


## Partition

partition LUKS ( chiffrée )

séparrer le tmp pour option de montage 


### option de montage 

nodev
nosuid   -> permet d'executer des droit avec des code 
noexec

suid permet d'executer qlq chose avec les meme droit que root 


## LVM / ajout disque 


## User

groupeadd students
useradd CuRs3d --badname -G Students -ms /bin/bash (or -d /home/student) -p (openssll  passwd -l toto)CuRs3d

usermod 

> /etc/skel 
**le contenue de se dosssier et copier lors de la création de nouveau user**

#### Commande créé user entierement
useradd --badname -m -d /home/curs3d -s /bin/bash -G students,cdrom,floppy,audio,dip,video,plugdev,users,netdev,bluetooth,lpadmin,scanner -p $(openssl passwd -1 toto) CuRs3d
 

> for num in {1..9};do useradd -u 200${num} -m -d /home/student${num} -G students -s /bin/bash -p $(openssl passwd -1 generic) student${num};done


## Droit/Permision

Chmod => permission sur un fichier/repertoir
chowon => change le owner (proprietaire) d'un fichier/repertoir
chgrp => change le grp owner d'un fichier

chown -R user fichier
chgrp -R user fichier

chown -R user:grp fichier 


## Commande en vraque

mkdir -p documentt/{cc,cc1]
whatch cat fichier 

sed -i 'ls/test/toto/g' fichier
sed -i '2aok' fichier

split pour separer un ficher par taille 

watch = voir a jour
## a regardeer

rfkill
lspci


propsmoke for esxi 
next cloud 
open media

demander a prodiox pour la commande jobs/affichier tout les proccessus 
