## Définition
Un $\mathbb{K}$-espace vectoriel est un [[Structure de groupes|groupe]] commutatif tel que :
$$
\begin{split}
(a+b)u &= au + bu \\
a(u+v) &= au + av \\
a(bu) &= (ab)u \\
1u &= u

\end{split}
$$
Les éléments d'un espace vectoriel sont appelés des **vecteurs**. Il ne sont pas forcements des n-uplets de $\mathbb{R}$, mais il est courant de s'y ramener.  
On note souvent un espace vectoriel de la manière suivante : $(E, +, \cdot)$.

## EV Produit
Soit deux espaces vectoriels, on peut les "additionner", permettant d'obtenir un nouvel espace vectoriel, comportant toutes les combinaisons linéaires des vecteurs des deux EV d'origines.
Si deux sev additionnés valent $E$, on dit qu'ils sont **complémentaires** dans $E$.
On dit que $F$ et $G$ sont en **somme directe** si $F \cap G = \{0_E \}$. Si $F$ et $G$ sont et complémentaires et en somme directe, on dit qu'ils sont **supplémentaires**.  
## Sous-espace vectoriel

^48cd3c

Soit $F$ une partie de $E$, si :
$$
\begin{align}
0_E &\in F \\
(x,y) \in F^2 &, \lambda x+y \in F
\end{align}
$$
On appel alors $F$ un sev (sous espace vectoriel) de $E$. 
Pour généré ces SEV, on utilise des familles de vecteurs. On les écrit comme suit :
$$
Vect(x_1, x_2, x_3, ..., x_n) = \{ax_1 + bx_2 ...\}
$$
Soit une famille de vecteurs de $E$, on la dit **libre** si ses vecteurs sont **linéairement indépendants**, c'est a dire, qu'il n'existe pas de combinaisons linéaires des premiers vecteurs qui amènent au dernier. Sinon, on dit que la famille est **liée**.

## Base
Une famille de vecteurs est appelé **base** si elle est a la fois **génératrice** et **libre**.
De toute famille génératrice de $E$ on peut extraire une base, et toute famille libre peut être complétée en une base. 
Soit $n = dim(E)$, toute famille libre a $n$ éléments est une base de $E$, et toute famille génératrice de $n$ éléments est une base. 

## Dimension
Quelques règles :
- $dim(F \oplus G) = dim(F) + dim(G)$
- $dim(F+G) = dim(F)+dim(G) - dim(F \cap G)$
- $dim(E \times F) = dim(E) + dim(F)$
## Rang
On appel le **rang** du famille la dimension de l'espace vectoriel engendré par cette famille. 