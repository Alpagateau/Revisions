## Définition
On appel le graph d'une relation, noté $R$ est un ensemble de tuples d'éléments de d'un [[Ensembles|ensemble]] $E$. On dit que deux éléments de $E$ sont en relations si $R$ contient un tuple de ces deux éléments. On le note alors $x \mathcal{R} y$.

Une relation peut avoir plusieurs propriétés :
- **Réflexivité** : $x \mathcal{R} x$
- **Symétrie** : $x \mathcal{R} y \Rightarrow y \mathcal{R} x$
- **Transitivité** : $x \mathcal{R} y, y \mathcal{R} z \Rightarrow x \mathcal{R} z$
- **Antisymétrie** :  $x \mathcal{R} y, y \mathcal{R} x \Rightarrow x = y$
## Relation d'équivalence
Une relation ($\mathcal{R}$) est dite d'**équivalence** si elle est a la fois **réflexive, symétrique et transitive**. Pour une telle relation, on défini pour chaque élément de $E$ une **classe d'équivalence**, noté $\mathcal{C}(x) = \dot x = \{y \in E, y \mathcal{R} x \}$.
Les classes d'équivalences forment une [[Ensembles#^partition|partition]] de $E$. L'ensemble des classes d'équivalences s'appelle l'**ensemble quotient** de $E$ par $\mathcal{R}$ noté $E / \mathcal{R}$.

## Relation d'ordre
> Cela se rapproche de la majoration pour les [[Fonctions de la variable réelle]]. 

Une relation ($\mathcal{R}$) est dite **d'ordre** si elle est **réflexive**, **antisymétrique** et **transitive**. Un ensemble muni d'une telle relation est dit ordonné. Les exemples les plus communs sont $\le$ et $\ge$. 
Soit A une partie de E non vide, on dit que $a$ est: 
- un **majorant** : $\forall x \in A, \quad x \le a$
- un **minorant** : $\forall x \in A, \quad x \ge a$
De plus, $a$ est un **extremum** si $a \in A$. On le note alors $max(A)$ (resp. $min(A)$). 
Si $A$ est admet un minorant et un majorant, on dit que $A$ est **bornée**. 

