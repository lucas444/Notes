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

## Fichier :

```py

f = open("flag.txt","r")
print(f.read())




f = open("demofile1.txt", "a") # Append to an existing file
f.write("The file will include more text..")
f.close()

f = open("demofile2.txt", "w") # Creating and writing to a new file
f.write("demofile2 file created, with this content in!")
f.close()

```
