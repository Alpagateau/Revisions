#somme #produit #télescopage
## Notations
$\displaystyle \sum_{k=0}^n a_k$   ce note `\displaystyle \sum_{k=0}^n a_k`
$\displaystyle \prod_{k=0}^n a_k$   ce note `\displaystyle \prod_{k=0}^n a_k`

$k$ est un indice. Les produits et les sommes peuvent aussi être représenté avec des [[Ensembles|ensembles]]. dans ce cas, la somme n'est pas indexée. 

## Propriétés

Les sommes sont linéaires 
$$
\displaystyle \sum_{k=0}^{n}(\lambda a_k + \mu b_k) = \lambda \sum_{k=0}^{n}a_k + \mu \sum_{k=0}^n b_k
$$
Les produits de sommes
$$
\displaystyle (\sum_{k=0}^n a_k)(\sum_{i=0}^m b_i) = \sum_{k=0}^n (\sum_{i=0}^m a_k b_i)
$$
Les facteurs d'un produits se regroupent
$$
\prod_{k=0}^n(a_k b_k) = (\prod_{k=0}^n a_k)(\prod_{k=0}^n b_k)
$$
## Changement d'indice
Si une somme ou un produit est indexé, on peu effectuer un changement d'indice.
C'est a dire, réécrire la meme somme (ou produit) sans en changer les termes (ou facteurs)

## Télescopage
L'idée est de simplifier la somme (ou produit) en faisant apparaître des termes s’annulant.
Par exemple :
$$
\sum_{k=m}^{n-1} (z_{k+1} - z_{k}) = 
(\sum_{k=m}^{n-1} z_{k+1}) - (\sum_{k=m}^{n-1} z_{k}) =
(\sum_{k=m+1}^{n} z_{k}) - (\sum_{k=m}^{n-1} z_{k}) = z_n + 0 -z_m
$$
## Résultats classiques
avec $(a,b) \in \mathbb{R}^2$ et $n \in \mathbb{N}^*$

- $\displaystyle \sum_{k=1}^n k = \frac{n(n+1)}{2}$
- $\displaystyle \sum_{k=1}^n k^2 = \frac{n(n+1)(n+2)}{6}$
- $\displaystyle \sum_{k=1}^n k^3 = \frac{n^2 (n+1)^2}{4}$
- $\displaystyle \sum_{k=1}^n a^k = \frac{1-a^{n+1}}{1-a}$
- $a^n - b^n = (a-b)\displaystyle \sum_{k=0}^{n-1} a^{n-1-k} b^k$
## Sommes doubles
Une somme double est une somme utilisant deux indices.
$$
S = \displaystyle \sum_{i \in I, j \in J} a_{ij}
$$
On peut la comparer a du code sous la forme :
```python
S = 0
for i in I:
	for j in J:
		S += a[i][j]
```
## Somme triangulaire
Une somme triangulaire est une somme double dont le second indice est limité par le premier. On l'appel ainsi car on peut représenter cette somme comme la somme d'une [[Matrices#^9149b2|matrice triangulaire]]. 

$$
\displaystyle S = \sum_{0 < i \le j \le n} a_{ij}
$$
$$
\displaystyle
\begin{pmatrix}
a_{11} & a_{12} & a_{13} & a_{14} \\
a_{21} & a_{22} & a_{23} & a_{24} \\
a_{31} & a_{32} & a_{33} & a_{34} \\
a_{41} & a_{42} & a_{43} & a_{44} \\
\end{pmatrix}
\rightarrow
\begin{pmatrix}
a_{11} & a_{12} & a_{13} & a_{14} \\
. & a_{22} & a_{23} & a_{24} \\
. & . & a_{33} & a_{34} \\
. & . & . & a_{44} \\
\end{pmatrix}
$$
En code
```python
#n un entier
S = 0
for i in range(1, n):
	for j in range(i, n):
		S += a[i][j]
```
## Somme par partition
Si on veux sommer tous les elements d'un ensemble $E$, on peut sommer les éléments d'une [[Ensembles#^561e54|partition]] de $E$. 
Ainsi, en utilisant les sommes triangulaires comme exemples :
$$
\displaystyle S = (\sum_{0 < i \le j \le n} a_{ij}) + 
(\sum_{0 < j < i \le n} a_{ij})
= \sum_{0 < j , i \le n} a_{ij}
$$
