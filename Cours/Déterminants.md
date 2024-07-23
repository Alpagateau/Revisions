#algebra
## Définition
Le **déterminant** est un nombre que l'on peut associer a une [[Matrices|matrice]] carrée (par extension, aux [[Applications linéaires|applications linéaires]]) et qui nous donne certaines informations sur cette matrice. 
On admet une interprétation géométrique des déterminant comme le "volume à  n-dimensions" du solide créer pas les vecteurs colonnes formant cette matrice. 
> Ce que j'appel le "volume a n-dimension" est l'extension du principe de volume aux dimensions supérieures et inferieur. Par exemple, c'est l'aire en 2D, le volume en 3D, etc...


![[Area_parallellogram_as_determinant.png|400]]  
## Notation
Soit $A$ une matrice carrée, on note alors le déterminant de $A$:
$$
det(A) = |A| = \begin{vmatrix}
a_{11} & a_{12} & ...\\
a_{21} & a_{22} & ... \\
...    & ...    & ...

\end{vmatrix}
$$
## Calcul
Pour une matrice de dimension $2\times 2$, la formule est la suivante :
$$
\begin{vmatrix}
a & b \\
c & d \\
\end{vmatrix}
= ad - bc
$$
Pour toute matrice carrée de dimension supérieure a $2 \times 2$, la formule est la suivante : 
$$
\displaystyle
det(A) = \sum_{k=1}^n (-1)^{k+1} a_{k,1} \times det(A_{k,1})
$$
avec $A_{i,j}$ est la matrice $A$ dont on a enlevé la ligne $i$ et la colonne $j$. En somme, cet une formule récursive.
Pour mieux comprendre l'algorithme, en voici une traduction en code 
```python
n = 10 #dimension de A
A = np.arrange((n,n)) #on initialise une matrice de dimension n*n

def det(M):
	p,q = M.shape
	s = 0 #somme
	for i in range(1,p+1): #on itère sur chaque ligne
		s += (-1)**(k+1) 
			* M[i,1] 
			* det(M.copy().delete(k,0).delete(1,0)) #A_{k,1}

```
## Multi linéarité
Le déterminant est **multilinéaire**, c'est a dire qu'il est linéaire a **chacune de ses colonnes**. 
c'est a dire :
$$
\begin{vmatrix}
\lambda a & \mu b \\
\lambda c & \mu d \\
\end{vmatrix}
= \lambda
\begin{vmatrix}
 a & \mu b \\
 c & \mu d \\
\end{vmatrix}
= \lambda \mu
\begin{vmatrix}
 a & b \\
 c & d \\
\end{vmatrix}
$$
## Règles sur le déterminant
1. Si deux vecteurs colonnes constituants la matrice sont colinéaires, le déterminant est nul
2. Si deux colonnes sont permutées, le signe du déterminant s'inverse
3. Le déterminant de la [[Matrices#^7c9416|transposée]] est le même. 
> La 3eme règle permet de développer le déterminant par colonne ou par ligne. 

## Méthodes de calculs a retenir
1. Multiples de matrices :
$$
det(\lambda A) = \lambda ^n det(A)
$$
2. Additions de lignes :
$$
det(A) = det(A'), \quad A'_{i,j} = A_{i,j} + A_{i_j+h}, i = cst, j \in [\![1, n]\!] 
$$
3. Multiplicité
$$
det(AB) = det(A)det(B) = det(BA)
$$
4. Matrice triangulaire ou diagonale :
$$
det(D) = \prod_{i=1}^n D_{i,j}
$$
5. Inverse :
$$
det(A^{-1}) = {1 \over det(A)}
$$

## Utilisation
Le déterminant peut servir a savoir si une matrice est inversible. En effet, celle-ci est inversible si et seulement si le déterminant est non nul. Dans ce cas, on calcul l'inverse avec la formule suivante :
$$
A^{-1} = {1 \over det(A)}com(A)^T
$$
avec 
$$
com(A)_{i,j} = (-1)^{i+j} * det(A_{i,j})
$$
