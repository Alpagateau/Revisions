## Définition
Soit une [[Suites numériques|suite]] $(u_n)_{n \in \mathbb{N}}$, on appel **série** (ou **somme partielle**)  la suite $S_n$ tel que 
$$
\displaystyle
S_n = \sum_{k=0}^n u_k
$$
Si (et seulement si) $S_n$ admet une limite finie, on note $\sum_{k=0}^{+\infty} u_k$ la somme de la série. On dit alors que la série est **convergente**. Sinon, elle est divergente. 
>Si la série est a terme dans $\mathbb{C}$, il faut que sa partie réelle ET sa partie complexe converge pour que la série converge. 
-------
>Pour que $S_n$ soit convergente, il faut que $u_n$ tende vers 0. Cette condition est nécessaire mais non suffisante !

Soit $S_n$ une suite convergente, on appel **reste d'ordre n** la série $R_n = \sum_{k=n+1}^{+\infty} u_k$. On as alors $\lim_{n \to +\infty} R_n = 0$. 
On a aussi que les séries convergentes sont stables par combinaisons linéaires. 

## Série a termes positifs
On appel série a termes positifs une série dont tous les termes sont positifs. 
Une tel série est obligatoirement croissante. Ainsi, elle converge seulement si celle ci est majorée. 

#### Théorème de comparaison
Soient deux suites $u_n$ et $v_n$ tel que 
$$
\exists k_0, \forall k \ge k_0, u_k \ge v_k
$$
Alors :
- $\sum u_k$ converge $\Rightarrow$ $\sum v_k$ converge
- $\sum v_k$ diverge $\Rightarrow$ $\sum u_k$ diverge

#### Théorème des équivalents
Soient $u_n$ et $v_n$ deux suites tel que $u_n \sim v_n$ [^1] alors elles ont la même convergence. 

#### Théorème de comparaisons suites / intégrales
Si il existe une fonction $f$ tel que $Im(f) \subset \mathbb{R}^+$ et $f$ décroissante sur $\mathbb{R}$,
alors :
$$
\displaystyle
\sum_{k=0}^{+\infty} f(k) \quad converge \quad \Leftrightarrow \quad \lim_{n\to +\infty}\int_{0}^{n} f(x)dx \quad converge
$$
#### Règles de Reimann
- si $a > 1$, et $\lim_{k \to +\infty} k^a u_k = 0$ alors $\sum u_k$ converge
- si $a \in [0, 1]$ et $\lim_{k \to +\infty} k^a u_k = +\infty$ alors $\sum u_k$ diverge

### Les différents types de séries
Il existes différentes séries remarquables. 
1. Les [[Série de Reimann]]
2. Les Séries géométriques de la forme $\sum q^k$

Les séries géométriques convergent si, et seulement si, la raison $q$ est tel que $|q| < 1$ On a alors :
$$
\sum q^k = {1 \over1-q}
$$

#### Règle de d'Alembert
Tout comme la règle de Reimann est une extension des [[Série de Reimann]], la **règle de d'Alembert** est une extension des règles des séries géométriques. On a alors :
avec $l = \lim_{n\to +\infty}{u_{n+1} \over u_n}$, 
- si $l < 1$ , $S$ converge
- si $l > 1$, $S$ diverge
- si $l = 1$, on ne peut pas déduire




[^1]: voir [[Comparaisons locale de fonctions#Equivalence|équivalence]] 