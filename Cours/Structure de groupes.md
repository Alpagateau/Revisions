#algebra 
## Définition
On appel un **groupe** un [[Ensembles|ensemble]] ($G$) muni d'une [[Loi de composition|loi de composition interne]] ($*$) tel que :
- $*$ est associative
- $*$ admet un élément neutre
- $*$ est inversible
On appel **abélien** un groupe tel que $*$ est **commutatif**.
On appel aussi **groupe symétrique** de $E$ l'ensemble des permutations (bijections), noté $\mathcal{Q}_E$.

## Sous groupe
On appel $H$ un sous groupe si $H \subset G$ et :
- $1_G \in H$
- $x*y^{-1} \in H$ 

## Morphisme
Soient $(G, *)$ et $(G', \Delta)$ deux groupes, $f$ est un morphisme ssi : 
$$
f(x*y) = f(x) \Delta f(y)
$$
On a alors:
$$
f(e_G) = e_{G'} \quad f(x^{-1}) = (f(x))^{-1}
$$

Un **endomorphisme** est un morphisme de $G$ dans $G$.
Un **isomorphisme** est un morphisme bijectif.
Un **automorphisme** est un endomorphisme bijectif.
