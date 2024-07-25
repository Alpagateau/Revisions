#algebra 
## Définition
On appel $I$ un **intervalle** de $\mathbb{R}$, si $I \subset \mathbb{R}$ et :
$$
\forall(x,y) \in I^2, \forall z, x \le z \le y \Leftrightarrow z \in I
$$
On dit d'un intervalle qu'il est :
- **fermé** : $[a,b]$
- **ouvert** : $]a,b[$
- **semi-ouvert** : $[a, b[$
- **demi-droite** (ouverte et fermée): $[a, +\infty[$  et  $]a, +\infty[$

De même, on appel **voisinage** d'un réel $x$, un intervalle $V$ tel qu'il existe un intervalle $O$ ouvert $O \subset V$ et $x \in O$
Dans la pratique, on considère le voisinage de $x$ un intervalle arbitrairement petit autour de $x$. 
> Un intervalle ouvert est un voisinage de tous ses points

## Intérieur et adhérence
Soit un intervalle $I = [a,b[$
On appel l'**intérieur** de $I$ ( $\displaystyle \mathring{I}$ ) l'ensemble des points de $I$ tel que $I$ est un voisinage de ce point. Dans les faits, si $I$ est fermé, $\mathring{I}$ est ouvert.
Dans notre exemple : $\mathring{I} = ]a,b[$
On appel l'**adhérence** de $I$ noté $\overline I$ l'ensemble des points $x$ de $\mathbb{R}$ tel que, pour tout voisinage $V_x$ de $x$, $V \cap I \ne \emptyset$.
Dans les faits, si $I$ est ouvert, $\overline I$ est fermé. Dans notre exemple, $\overline I = [a,b]$. 
> Un point $x$ est dans l'adhérence de $I$ si et seulement si, il existe une suite d'éléments de $I$ dont la limite est $x$

---

Toute [[Ensembles|partie]] de $\mathbb{R}$ est [[Relation binaire#Relation d'ordre|ordonée]] par la relation $\le$.
- Toute partie non vide de $\mathbb{R}$ majorée admet une borne supérieure.
- Toute partie non vide de $\mathbb{R}$ minorée admet une borne inférieure.
