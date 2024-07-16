## Fonction négligeable
On dit que $f$ est **négligeable** en $a$ devant $g$ si :
$$
\displaystyle \lim_{x \to a} \frac{f(x)}{g(x)} = 0
$$
On écrit alors 
$$
f = o_a(g) \quad ou \quad f <<_a g
$$
La [[Relation binaire|relation]] de négligeabilité est **transitive**, et stable par combinaison linéaire ainsi que par produit.  
Quelques exemple de fonctions négligeables :
- $x^a = o_0(x^b) \Leftrightarrow a > b$ 
- $x^a = o_{+ \infty}(x^b) \Leftrightarrow a < b$
- $ln^a(x) = o_{+ \infty}(x^b)$
- $x^b = o_{+ \infty}(e^{cx})$

## Fonction dominée
On dit que $f$ est dominée par $g$ si:
$$
\exists \epsilon, \forall x \in \overline a,  \mid\frac{f}{g}\mid < \epsilon
$$
On le note $f = O_a(g)$. Cette notation est très utilisé en informatique pour représenter la complexité des algorithmes. ![[Big_O_Complexity.png]]