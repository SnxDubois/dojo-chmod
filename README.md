# Chmod

Vous avez en entrée une chaîne de caractère composées de 3 chiffres compris entre 1 et 7.
Vous devez définir quelles sont les autorisations accordées en fonction.

```
Ex: 145
```

Chaque chiffre composant la chaîne nombre se décompose ensuite en binaire :

```
Ex: 001 010 101
```

À chaque groupe de trois chiffre binaire est associée la suite de droit correspondant : read (r), write (w), execution (x).
On associe la lettre si c'est un 1, et un tiret si c'est 0. On colle ensuite tous les caractères ensemble.

Ex: --x-wr-x

* [chmod by the Numbers](https://catcode.com/teachmod/numeric.html)

```
Ex:
    Entrée : 000, Sortie : ---------
    Entrée : 124, Sortie : --x-w-r--
    Entrée : 777, Sortie : rwxrwxrwx
```

Rappel des commandes junit :

```
javac -cp .:junit-4.12.jar ChmodTest.java
java -cp .:junit-4.12.jar:hamcrest-core-1.3.jar org.junit.runner.JUnitCore ChmodTest
```
