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