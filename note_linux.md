# Text-FU

## stdout
Sortie 0

```bash
echo hello word > hello.txt
# > envois le stdout dans le fichier
```
\> write
\>> add 


## stdin
sortie 1

```bash
cat < hello.txt > banana.txt
# affiche se qu'il y a dans hello.txt et le copie dans banana
```

## stderr
sortie 2

```bash
ls /fake/directory > erreur.txt 2>&1
# renvois l'erreur de la commande dans le fichier erreur.txt

ls /fake/directory 2>&1 peanuts.txt
# renvois l'erreur ET LA SORTIE STANDARD (stdout) dans le fichier erreur.txt

ls /fake/directory &> peanuts.txt
```




