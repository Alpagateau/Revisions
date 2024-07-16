## Vocabulaire
Une **proposition** est un énoncé vrai ou faux. On note V et F (ou 1 et 0) les valeurs logiques.

## Opérations
Soient $P$ et $Q$ deux propositions, on definie :
- La **négation** : $non \space P = \overline{P}$
- La **disjonction** : $P \space ou \space Q = P \lor Q$
- La **Conjonction** : $P \space et \space Q = P \land Q$
- L'**implication** : $P \Rightarrow Q$
- l'**équivalence** : $P \Leftrightarrow Q$

## Negation avec quantificateurs
Lors de la negation d'une proposition, les quantificateurs changes, de meme que les symboles logiques. Ainsi, 
- $\exists \rightarrow \forall$ 
- $\forall \rightarrow \exists$
- $P \rightarrow \overline{P}$
- $(P \Rightarrow Q) \rightarrow (P \land \overline{Q})$

## Point de vue ensembliste
Soit $P(x)$ et $Q(x)$ deux propositions dépendants de $x$, un élément d'un [[Ensembles|ensemble]] $E$.
On note $$ A = \{x \in E, P(x) = 1\}, \space \space B = \{x \in E, Q(x) = 1\}$$
On as alors:
- $P(x) \Leftrightarrow x \in A$ 
- $P(x) \lor Q(x) \Leftrightarrow x \in A \cup B$
- $P(x) \land Q(x) \Leftrightarrow x \in A \cap B$
- $P(x) \Rightarrow Q(x) \space \Leftrightarrow A \subset B$
- $P(x) \Leftrightarrow Q(x) \space \Leftrightarrow A = B$

De plus tous les [[Ensembles#^loisurlesensembles| lois sur les ensembles]] s'appliquent aux propositions. 