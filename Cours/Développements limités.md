#calculus 
>Ce chapitre ne traite pas des [[Développements généralisés]].
## Définition
Un **développement limité** (DL) est une approximation [[Polynomes|polynomiale]] de fonctions au voisinage d'**un point**. Si une telle approximation existe, elle permet de lever certaines indéterminations lors de calculs de limites, ainsi que de simplifier l'[[Comparaisons locale de fonctions|étude locale de fonctions]].
Un exemple serait l'**approximation des petits angles** qui indique que pour un angle $\theta$ proche de zéro, $cos(\theta)$ vaux 1  et $sin(\theta)$ vaux $\theta$.
Cette approximation **locale** conserve la parité de la fonction. 
## Notation
Un DL a l'ordre $n$ en $x_0$, s'il existe, se note donc $DL_n(x_0) \space de \space f$, et on cherche donc un polynôme $P(x)$ tel que, au voisinage de $x_0$ :
$$
f(x) = P(x-x_0) + o_{x_0}(x^n)
$$
avec $o_{x_0}(x^n)$ une fonction [[Comparaisons locale de fonctions#Fonction négligeable|négligeable]] devant $x^n$.  
Le plus souvent, on considère le DL en 0. 

## Existence et Unicité
Un $DL_{n}(x_0)$ existe si et seulement si $f$ est continue en $x_0$ et dérivable $n$ fois. On utilise ensuite la [[Formules de Taylor|formule de taylor-young]] pour obtenir le DL.
Si un $DL_n$ existe, il est unique (sa partie polynomiale est unique) et tout $DL_p$ avec $p < n$ existe. 
Si $f$ admet un $DL_n$, alors toute primitive $F$ et $f$ admet un $DL_{n+1}$ trouvable par intégration de la partie 
Si $f$ admet un $DL_n$, alors $\displaystyle 1 \over f$ en admet un aussi. Dans la pratique, on considèrera le plus souvent $1 \over {1 + u}$ avec $u = f-1$. 

## Opérations
Les $DL_n$ sont stables par combinaisons linéaires. Ils sont aussi stables par produits, avec leurs résultats tronqué au rand $n$. 
7862 5620

## DL Usuels
Tous les DL montrés ici sont en 0. De plus, cette liste est une version simplifier. Pour certaine formule, notamment celle de $1 \over 1+u$, il suffit de prendre $-u$ et de prendre en compte la parité de la puissance. De même, ce tableau est présenté avec un réel $x$ mais il est le même pour les DL composés

| Fonction      | DL d'ordre n                                                              |
| ------------- | ------------------------------------------------------------------------- |
| $e^x$         | $1+x+{x^2 \over 2!} +{x^3 \over 3!}+ ... +{x^n \over n!} + o(x^n)$        |
| $cos(x)$      | $1 - {x^2 \over 2!} + {x^4 \over 4!} ... + o(x^n)$                        |
| $sin(x)$      | $x - {x^3 \over 3!} + {x^5 \over 5!} + ... + o(x^n)$                      |
| $(1+x)^a$     | $1 + ax + {a(a-1) \over 2!}x^2 + {a(a-1)(a-2) \over 3!}x^3 + ... +o(x^n)$ |
| $1 \over 1-x$ | $1 + x + x^2 + x^3 + x^4 ... + o(x^n)$                                    |
| $ln(1-x)$     | $-x - {x^2 \over 2} - {x^3 \over 3}+ ... + o(x^n)$                        |
