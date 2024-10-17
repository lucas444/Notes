# Cour théorique

chiffrement de vernam -> incassable matématiquement mais trop lourd


## Chiffrement par bloc
chiffre par bloc de donner ( taille) bloc de 128 
`exemple = train , ajout d'un vagon si trop d'utilisateeur`
ex:  des
AES chiffrement du cpu (modifer par la NSA/ téorie du complo du prof )

ECB
CBC
CTR
gc -> galois counter mode

## Chiffrement par flux
def : autant d'octer en entrer que en sortie 

RC6

wop facile a casser 



chffrement assimétrique 2 echange :
envois chiffrer alice
renvoi chiffrer bob
dechif allice
dechiffre bob
bob a les data


## Hash  
calcul unique
tail de l'antrer est fix 

est iréversible 


problématique de colition de hash : pas d'infinie de sortie 

check sam : paritter du bit != au check sam 

exemple SHA1-3 - MD5 - Argon2 et ploy???

## PBKF 
Sécuriter pour autentification des pwd 

## PKI
= signatre d'un certificat par un autre certificat

non répudiation 

### Standar :

PCI DSS (payement en ligne )
FIPS

international 
ISO / 
NIST

### Régulation
US : ferpa et hipaa 
eu : GDPR/ rgpd
fr : ANSSI

# Application de chiffrement : 

## librérie de chiffrement

OpenSSL/LibreSSL

Stocke tout les algo de chiffrement


## protocole ethernet 
802.1X

### wifi 
wop -> obselet 
wpa2-3 


serveur radius authent avec certificat 

### Open VPN
IPSEC / SSL

WireGuard

ciffrement de bout en bout uniquement l'utilisateur et le clientpeux dechiffrer


### OPEN SSH/SFTP

Chiffrer l'acces distant 

### DNSSEC & DNSCrypt

signature des dns sec

DNSSEC authentifi les requete

## Kerberos

ticketing / gestion des accès

optenir le hash d'un pass puis brut force
golden ticket = créé des ticket pour faire nimp ( demande les dtoid ad) 


### chiffrement de mail 

ancienement PGP 
mtn protimaill ou tutanot

faile = efail avec du javascript

### ssl/tls https & hsts/hpkp

https = http + ssl/tls

attck : ssl strip


### darknet

tor/ I2P


## Cryptocurencies & blockchain


les mineur brut force le hash pour retrouver le hash du block 


## TDE/TPM/HSM/DRM

HSM équipement phisique de chiffrement 
TPM chiffrement ordi -> hash puis stock l'os, bios, ....
bitlocker chiffrement de disque dur -> disque recovery en clair -> stocket la clé dans tpm



## File/disk Encryption

luks/ bitlocker = chiffrement ms ou linux

trueCrypt 
veraCrypt -> chiffre un disque dur virtuel 

mbr/gpt partition de boot boot loader en claire pas chiffrer 

## distribution quanum key

machine de turing 
quantique est probabiliste


## exploit

### AES-128-CBC modification
on peux modifier un bloc en xoran avec le précédent.

### logiciel 

- Burp 

- Mitmproxy
py -> perment de donner le trafic de la machine en claire pour du script py 



