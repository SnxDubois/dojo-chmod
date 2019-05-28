# Chmod

Vous avez en entrée une chaîne de caractères composée de 3 chiffres, chacun compris entre 0 et 7.

Vous devez définir quelles sont les autorisations accordées, en fonction de l'entrée.

```
Ex: 142
```

Chaque chiffre de la chaîne se décompose en nombre binaire :

```
Ex: 001 100 010
```

Chaque nombre binaire est ensuite associé au droit correspondant : read (r), write (w), execute (x).

Une lettre est associée au 1 et un tiret au 0. Les caractères sont ensuite concaténés.

```
Droits:   rwxrwxrwx
Binaire:  001100010
Résultat: --xr---w-
```

* [chmod by the Numbers](https://catcode.com/teachmod/numeric.html)

```
Ex:
    Entrée : 000, Sortie : ---------
    Entrée : 352, Sortie : -wxr-x-w-
    Entrée : 777, Sortie : rwxrwxrwx
```

Rappel des commandes junit :

```
javac -cp .:junit-4.12.jar ChmodTest.java
java -cp .:junit-4.12.jar:hamcrest-core-1.3.jar org.junit.runner.JUnitCore ChmodTest
```
