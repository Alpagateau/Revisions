#algebra 
## Definition
Une matrice est un tableau d'éléments, appelés coefficients, appartenant a un ensemble $\mathbb{K}$. On note $\mathcal{M}_{n,p}(\mathbb{K})$ l'ensemble des matrices de taille $n \times p$ avec $n$ le nombre de lignes et $p$ le nombres de colonnes. Si $p = n$, on peut noter $\mathcal{M}_n (\mathbb{K})$. On appel ces matrices **carrées** de taille $n$. Une matrice **carrée** est dite **diagonale** si seuls les coefficients de position $(i,j), i=j$ soient non nuls.  

Une matrice **carrée** est dite **triangulaire** si seuls les coefficients de position $(i,j), i \ge j$ soient non nuls.  ^9149b2

On appel une matrice **élémentaire** si elle ne possède qu'un seul coefficient non nul, et que celui ci vaux $1$  

La **base canonique** d'une matrice est une famille de $n \times p$ matrices élémentaires, tel que chacune ai son $1$ a une position différente. 

Soit $A$ une matrice, on note $A^T$ la transposé, cet a dire le miroir par la diagonale, de la matrice A.  ^7c9416

On note $0$ ou $0_{n,p}$ la matrice de taille $n \times p$ dont tous les coefficients sont nuls. 
On a que $\mathcal{M}_{n,p}(\mathbb{K})$ est un $\mathbb{K}$-[[Espace vectoriel|espace vectoriel]] d'élément neutre 0. ^d59392

## Opérations
##### Multiplication par un scalaire
$$\lambda A = \begin{pmatrix} \lambda a_{11} & \lambda a_{12} \\   \lambda a_{21} & \lambda a_{22}\end{pmatrix}$$

##### Addition
$$
A + B = \begin{pmatrix} a_{11} + b_{11} & a_{12} + b_{12} \\
a_{21} + b_{21} & a_{22} + b_{22} \end{pmatrix}
$$

##### Produit matriciel

Soient $A \in \mathcal{M}_{n,p}(\mathbb{K})$ et $B \in \mathcal{M}_{p,q}(\mathbb{K})$

$$
\displaystyle
\forall(i,j) \in [\![1,n]\!] \times [\![1,q]\!], c_{i,j} = \sum_{k=1}^p a_{i,k}b_{k,j}
$$
En code, on écrirai :
```python
A = #2d array n*p
B = #2d array p*q
C = #empty 2d arrays n*q

for i in range(n):
	for j in range(q):
		for k in range(p):
			C[i,j] += A[i, k] * B[k, j]
```

Le produit matriciel n'est **pas commutatif**. Par contre, on lui reconnais les propriétés suivantes : 
- **Associativité** : $(AB)C = A(BC)$
- **Distributivité de chaque coté** : $(\lambda A + \mu B)C = \lambda AC + \mu BC$ 
- **Element neutre** : $I_n A = AI_p = A$

## Binôme de matrices
On suppose que $AB = BA$ avec $B$ et $A$ deux matrices. On peut alors utiliser le [[Binôme de newton]]. 
$$
\displaystyle
(A+B)^k = \sum_{j=0}^k \binom{k}{j} A^j B^{k-j}
$$
On obtiens aussi :
$$
\displaystyle
A^k - B^k = (A-B)\sum_{j=0}^{k-1}A^jB^{k-j-1}
$$
## Inverse
L'inverse d'une matrice $A$ est la matrice $B$ tel que $AB = BA = I_n$
On note $B = A^{-1}$. L'ensemble de toutes les matrices inversibles est appelé groupe linéaire, et est noté $GL_n(\mathbb{K})$. 
Pour inverser une matrice, on utilise l'algorithme de [[Pivot de Gauss|gauss-jordan]].

