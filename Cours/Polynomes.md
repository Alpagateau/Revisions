#algebra 
## Définition
La définition "réelle" des polynômes est la suivante :
Un polynôme est une [[Suites numériques|suite]] tel que tous ses termes sont nuls a partir d'un certain rang. Un polynômes tel que tous ses termes sont nuls est dit polynôme nul.
En réalité, on considérera plus souvent sa **fonction associée** qui est :
$$
\displaystyle
\tilde P(x) = \sum_{k=0}P_k \times x^k
$$
Par abus de language, on appellera **polynôme** cette fonction associée. 
Pour garder la généralité, on va posé un polynôme $X = (0, 1, 0, 0, ...)$. Ainsi, on écrit les polynômes comme somme de puissances de $X$. 
> $X$ est strictement différent de $x$. L'un est un polynôme, l'autre est une variable.

On écrira ainsi les polynômes de la manière suivante :
$$
P = (0, 5, 2, 2, 1, 0, 0, 0, ...) = 0 + 5X + 2X^2 + 2X^3 + X^4
$$

L'ensemble des polynômes se note $\mathbb{K}[X]$ avec $\mathbb{K}$ l'ensemble des réels ou des [[Nombres complexes|complexes]]. 
## Degré
On appelle **degré** ($deg(P)$) le rang du dernier terme non nul de P, ou plus simplement, la plus haute puissance de $X$ dans l'écriture de $P$. Le dernier terme non nul s'appel le **coefficient dominant**. Si le coefficient dominant vaux $1$, on dit le polynôme **unitaire**.
On as alors quelques propriétés :
- $deg(P+Q) \le max(deg(P), deg(Q))$ car leurs **termes dominants** peuvent s'annuler. 
- $deg(\lambda P) = deg(P)$
- $deg(P \times Q) = deg(P) + deg(Q)$
- $deg(P \circ Q) = deg(P) \times deg(Q)$
- $deg(P') = deg(P) - 1$


## Opérations
Les polynômes sont stables par combinaisons linéaires ainsi que par multiplication interne. La multiplication interne se fait par distributivité (ou produit de Cauchy). 
Les polynômes sont aussi stables par compositions. 
Il existes d'autre lois pour le [[Calcul Polynomial]]. 

