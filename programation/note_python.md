# Note Python

### Boucle While

```py
i = 1
while i <= 10:
     print(i)
     i = i + 1
```

### Boucle For 

```py
websites = ["facebook.com", "google.com", "amazon.com"]
for site in websites:
     print(site)

```


```py
for i in range(5):
     print(i)
```

## Manipulation des fichiers

###Lecture de fichier

```python

f = open("flag.txt", "r")
print(f.read())
f.close()  # Pensez à fermer le fichier après utilisation
```
###Écriture dans un fichier

- Ajout de texte à un fichier existant :

```python

f = open("demofile1.txt", "a")
f.write("Le fichier contient maintenant plus de texte.")
f.close()
```
- Création et écriture dans un nouveau fichier :

```python

f = open("demofile2.txt", "w")
f.write("Le fichier demofile2 a été créé avec ce contenu.")
f.close()
```

## type de données
```py
a ="hello word"
# string

b = 3.14
#float
```

### numérique
1. Entier
2. Flottans
3. Nombres

#### 1.Entier

```python
a = 25
b = -12345678

a + b
```

#### 2.Floantant
```py
a = 1.23
b = -2.25e14
#e exposant
```

#### 3.Numérique
```py
a = 2+3j 
# J = complexe
type(a) 
# connaitre le type de la variable
```

#### 4.Booléen

```python
a = True
# ok
b = true
# error

note (a)
# renvoi l'oposer de la valeur 
```

### Opérateur 


|Opérateur|Nom|
|---------|---|
|+|Adition|
|-|Soustration|
|*|Multiplication|
|/|division|
|%|Modulo|
|//|Reste|




|Opérateur|Exemple|Equivalent|
|---------|-------|----------|
|=|x = 5|x = 5|
|+=|x += 3|x = x + 3|
|-=|x -= 3|x = x - 3|
|*=|x *= 3|x = x * 3|
|/=|x /= 3|x = x / 3|
|%=|x %= 3|x = x % 3|
|//=|x //= 3|x = x // 3|
|**=|x **= 3|x = x ** 3|
|&=|x &= 3|x = x & 3|
|\|=|x \|= 3|x = x \| 3|
|^=|x \^= 3|x = x ^3|
|<<=|x <<= 3|x = x << 3|
|>>=|c >>= 3|x = x >> 3|



```python
a = 5
a += 5
# a = 10

```

### Chaine de caratère 

```py
b ="hello"
c = 'hello'

# pass 1 char mais une chaine donc :
b[1:2] = el

b.upper # maj (affichage)
b = b.lower #minuscule 
```

---

### liste :

```python
liste = [1,3,2]
liste.sorte()
# trie les ellement

liste.append([cc])
#ajout un ellement /une liste a la liste 

liste.extend(["a","b"])
# ajoute des élement a la liste 

liste.count(0)
#conte le nombre d'apparicion d'une valeur


