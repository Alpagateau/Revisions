#algebra 
## Définition
La **décomposition en éléments simples** (DES) est une méthode qui permet d'écrire toute [[Fractions rationnelles]] sous la forme d'une somme d'un [[Polynomes]] et de plusieurs **éléments simples**. Celle-ci est très utilisé dans le calcul d'[[Intégration|intégrale]] car elle permet de grandement simplifier la recherche de primitives.

## Élément simple
Un élément simple est une fraction rationnelle notée $\displaystyle \frac{J}{H^k}$ où $Q$ est [[Calcul Polynomial#^f4482d|irréductible]] et où $deg(J) < deg(H)$.  

## Ecriture formelle
Soit une fraction rationnelle $\displaystyle F = {P \over Q}$. On a que $Q$ est un produit de facteurs irréductibles (de la même manière que chaque entier est produit de facteurs premiers). On note ces facteurs $H_i$ tel que
$$
Q = \prod_{i=1}^n H_i^{m_i}
$$
>Pour garder en tête la comparaison avec les entiers, c'est l'équivalent d'écrire que $2^2 \times 3 \times 5^3 = 1500$. 

Il existe alors $E \in \mathbb{K}[X]$ appelé **partie entière**, équivalent au quotient de la division euclidienne de $P$ et $Q$. 
Il existe aussi $R_{i,k} \in \mathbb{K}[X]$ tel que $deg(R_{i,k} < k\times deg(H_i)$. 
Ainsi, la DES complète s'écrit 
$$
\displaystyle
F = E + \sum_{i=1}^n \sum_{k=1}^{m_j} {R_{i,k} \over H_j^k}
$$
# Méthode
on considère une fraction $\displaystyle F = {P \over Q}$ 
## I - Partie entière
Par définition, la partie entière le quotient de la division euclidienne de $P$ par $Q$. Soit $R$ le reste de cette division, on a alors :
$$
F = E + {R \over Q}
$$
## II - Recherche des coefficients
#### 1 - Pôle simple
On considère $a$ une racine **simple** de $Q$, alors on cherche une écriture de la forme :
$$
\lambda \over X - a
$$
Pour ce faire, on multiplie $F$ par $(X - a)$ puis on évalue en $a$. Ceci nous donne exactement $\lambda$. 
#### 2 - Pôle multiple
La méthode est similaire, bien qu'une différence est a noté. Ici, on considère $a$ une racine de multiplicité 2 ou plus. On a alors 
$$
F = E + {a_1 \over X-a} + {a_2 \over (X-a)^2} + ... + + {a_n \over (X-a)^n} + S
$$
avec $S \in \mathbb{K}(X), \space S(a) \ne 0$, la suite de la DES. 
La méthode est ensuite quasiment la même que pour les pôles simples. On détermine d'abord $a_n$ en multipliant $F$ par $(X - a)^n$. On évalue en $a$ pour obtenir $a_n$.
On soustrait alors $\displaystyle a_n \over (X-a)^n$ à $F$. On recommence pour $a_{n-1}$. 

## III - Autres méthodes
- Evaluer $F$ en quelques valeurs simple peu permettre de trouver des relation entre les coefficients.
- La pratique de multiplier par le dénominateur d'un élément simple peut aussi servir si le nominateur n'est pas un scalaire. 