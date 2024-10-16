# Commande
```
stat = donne les stat d'un fichier 
wc = word count (ligne, mots, octet)
du -h = disque usage (humain)
df = taille de tout les périférique
```
### permition
```bash
chmod root.root

chmod a+rw fichier/fichier = all ajout ecriture lecture
    a all 
    u utilisateur
    g groupe
    o otre

    -R = modifier toute les sous dossier 

chown -R root.root fichier/ = change le propriétaire du fichier

umask = 6 = lecture ecriture 
        7 = lecture ecriture execution
```

### find 
``` bash
find /home -name *.txt -print
find /home -path /home/*/ *.txt -print
find /home -iname "[pt]*.txt" -print 
    #iname expresion rationnelle
    #lname lien symbolique

find /home -name lucra -type f -print 
    #f = fichier
    #d = directory
    #l = lien

find . -amin 1
   # a = accéder
   # c = changer de status(exemple : permition )
   # m = modifier
     #time = jour
     #min = minute

find . -acnewer fstab -print
    #apres modification de fstab

find . -size 12k -print
find . -size +/-12k -print:

find . -empty -name source* -type f -print 
    #empty = vide
```

### Grep (recherche dans 1 fichier )
```bash
grep "^#" fstab
    #recherche que les ligne commence pas un # (regex)
    #-i non sensible a la case 
    #-v inverse la recherche
    #-c nombre de ligne 
    #-b numéro de la ligne 
    #-w mot complet 
    #-l nom du fichier
    #-R recircive

grep -iwRl "print" *

#egrep = syntaxe etendu expresion rationnelle
#fgrep = pas déxpresion rationelle (regex)
```

### globbing 

```bash
ls \x??*

#* = nimporte quoi
#? = 1 caractère
#\? = commence par un ?
#x = commence par x
#[xw] = plusieur caractère
#^x = inversion (ne dois pas etre x)
```


### Redirection
|Pointeur|STREAM|
|-----|---------------|
|stdin|Entrée standard|
|stdout|Sortie standard|
|stderr| Erreur standard|

```bash
ls -l > /homme/lucra/resulat
    #> recréé/écraser 
    #>> créé/ajout 
```

###PIPE
``` bash
ls | sort -r 
    #(trie)
    #-r = inverse
```

### Find bis

```bash
find ~ -type f -exec grep -il 'term' {} \;
find ~ -type f -print0 | xargs -0 grep -il 'term'
    #-print0 = (régle les pb si nom de fichier bizzare)
    # xargs = récupere les argument et les envois a une autre commande  
    #         convertie output en suite d'argument 

find ~ -type f -print0 ! -name '.*' | xargs -0 grep -il 'term'
    # ! -name ".*" négation de commence par un point

find ~ -type f -print0 ! -name '.*' | xargs -0 grep -il 'term'  | xargs rm

find / -type d -empty -print0 | xargs -0 r
```

### compresser/décompresser

```bash
# zip / gzip : algorite de compréssion/décompréssion

tar -czvf ploud.tar.gz # compresse
    # c = compréssion
    # z = gzip
    # v = visuel
    # f = fichier

tar -tzvf ploud.tar.gz # affiche le comptenue 
    # t = voir le comptenue

tar -xzvf plouf.tar.gz
    #x= extraire
```

## USER

> user{add, mod, del}
> group{add, mod,del}




