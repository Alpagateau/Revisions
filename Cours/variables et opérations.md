## Définition
Une **variable** est une case dans la mémoire d'un ordinateur, à laquelle on a donné un nom. C'est aussi simple que ça. 

## Types de variables
Une case de mémoire peut contenir pleins de choses différentes, comme un nombre, un text, un fichier, une connexion a un serveur... Mais toutes ces information restent en binaire, en 0 et 1. Pour savoir comment utiliser les infos dans cette case mémoire, on lui attribut un type. Les types principaux sont les suivants : 

| Type          | Genre de données                                        | Notation mathématique |
| ------------- | ------------------------------------------------------- | --------------------- |
| int / integer | entier, positif ou négatif                              | $\mathbb{Z}$          |
| float         | nombre a virgule                                        | $\mathbb{R}$          |
| bool          | vrai ou faux                                            | $\{0; 1\}$            |
| string / str  | une chaine de caractères / du texte                     |                       |
| list          | Une listes de valeurs, pouvant être de différents types |                       |
Il en existe bien d'autres....

> Python déduit tout seul quel type de variable vous essayez de créer. Il n'y a donc pas a trop s’embêter. 

## Exemple en Python
Ici on va juste créer une variable et obtenir son type. Voici un exemple  de code :
```python
a = 4

print(a)
print(type(a))
```
#### Que fait ce code ?
On nomme une variable `a` et on lui donne la valeur 4. On a alors un entier. Ensuite, la fonction `print` affiche la valeur de a, puis son type. 
Ici on obtient :
```bash
C:\Users\Examples\Code python script.py
4
Int
```

Essayez de changer la valeur de `a` pour obtenir différents types de variables. 
> Si vous obtenez une erreur, c'est très bien !! Lisez la, et aidez vous de google pour comprendre pourquoi votre code ne fonctionne pas !

