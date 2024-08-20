## Définition
Les **nombres quantiques** sont des valeurs permettant de définir l’état quantique d'un système. En plus simple, ce sont 4 variables qui permettent de définir chaque electron d'un atome. Ainsi, chaque electrons dans un atome peut être définit par un **unique** quadruplet. 

```cpp
class electron
{
public:
	unsigned int n;    //Nombre quantique principal
	unsigned int l;    //Nombre quantique azimutal
	int m_l;           //Nombre quantique magnétique
	bool spin;         //Nombre quantique magnétique de spin 
};
```

## Nombre quantique principal
Le premier nombre quantique, noté $n$ identifie la couche électronique où se situe l'électron. Celui correspond ainsi a son niveau d’énergie. 
C'est un entier positif. Ce nombre lié par les [équations de Schrodinger](https://fr.wikipedia.org/wiki/%C3%89quation_de_Schr%C3%B6dinger#Recherche_des_%C3%A9tats_propres) a la distance entre le noyau et l'electron. C'est de la que viens le terme **couche électronique**.

## Nombre quantique azimutal
Le second nombre quantique, noté $l$ indique la sous-couche dans laquelle se trouve l'electron. $l$ est un entier positif ou nul, strictement inférieur a $n$.
Ce nombre quantique permet de determiner l'angle de liaison avec d'autres atomes. Lorsqu'il vaut 0, 1, 2 ou 3, il porte alors les noms plus connus s, p, d et f[^1].

## Nombre quantique magnétique
Ce nombre, noté $m_l$ permet de completer la definition des **orbitales atomiques**. Physiquement, celui ci représente la projection de son moment angulaire sur un axe. 
Il peut prendre des valeurs entre $-l$ et $+l$ inclues. 
C'est de lui que provient le nombre d"électrons dans chaque sous couches. 
Ainsi, si $l$ vaux $0$ (on est dans la couche $s$), il n'y a qu'une seule orbitale. On pourra alors y mettre deux electrons (grace au spin).

## Nombre quantique magnétique de Spin
Le **spin** noté $m_s$ identifie l'electron dans son orbitale. Le spin peux prendre deux valeurs $-{1 \over 2}$ ou $+{1 \over 2}$.  


[^1]: Ces lettres proviennent de la façon dont les couches ont été découvertes. On a repéré des lignes sur le spectre de certains métaux, ce qui a donné les noms : *Sharp, Principal, Diffuse, Fundamental*. 