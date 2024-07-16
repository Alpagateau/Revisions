#arithmetic
## Definitions

^561e54

Un **ensemble** est une collections d'objets, appelés **éléments**. On note  $x \in E$ l'élément $x$ appartient a $E$. L'ensemble vide se note $\emptyset$. Un ensemble peu en contenir un autre, on le note $F \subset E$.  Si $E$ est un ensemble, on note l'ensemble de ses sous-ensembles $\mathcal{P}(E)$. Chaque sous-ensemble est alors appelé une **partie** de $E$. A noté que E et $\emptyset$ sont toujours des parties de $E$. De plus, on appel **partition**  un ensemble de sous-ensembles disjoints de $E$ tel que leurs union vale $E$
^partition
## Ecriture des ensembles
Ils existe deux manieres principales d'ecrire des ensembles:
- L'ecriture en extension : $\{1, 2, 3, 4 ,... \}$
- L'écriture en comprension : $\{ x \in \Bbb{R}, x^2 = 4 \}$ 

## Opérations entre ensembles
Soient $A$ et $B$ deux parties de $E$. ^3a3a61

| **Intersection** : $A \cap B$                                      | **Union** : $A \cup B$                                 |
| ------------------------------------------------------------------ | ------------------------------------------------------ |
| **Complementaire** : $\overline{A} = \mathcal{C}_E A$              | **Difference ensembliste**: $A \backslash B$           |
| **Difference symétrique** : $A \Delta B$                           | **Disjonction** $\Leftrightarrow A \cup B = \emptyset$ |
| **Produit Cartésien** : $E \times F = \{(x,y), x \in E, y \in F\}$ |                                                        |

## Lois sur les ensembles

^loisurlesensembles

Soient $A, B, D \subset E$ :
- $A \subset (A \cup B), B \subset (A \cup B), (A \cap B) \subset A, (A \cup B) \subset B$
- $A \subset B, B \subset A \Rightarrow A = B$
- **Associativité** : $A \cup (B \cup D) = A \cup B \cup D$ et $A \cap (B \cap D) = A \cap B \cap D$ 
- **Commutativité** : $A \cup B = B \cup A$ et $A \cap B = B \cap A$
- **Distributivité** : $A \cup (B \cap D) = (A \cup B) \cap (A \cup D)$ et $A \cap (B \cup D) = (A \cap B) \cup (A \cap D)$ 
- **Règles De Morgan** : $\overline{A \cap B} = \overline{A} \cup \overline{B}$  $\overline{A \cup B} = \overline{A} \cap \overline{B}$

## Cardinal
Pour un ensemble fini, le cardinal est le nombre délements de ensemble. Il est noté $Card(E)$.
Soient $E$ et $F$ deux ensembles disjoints, alors $$Card(E \cup F) = Card(E) + Card(F)$$
On peut generaliser cette loi, on obtiens :
$$Card(A \backslash B) = Card(A) - Card(A \cap B)$$
$$Card(A \cup B) = Card(A) + Card(B) - Card(A \cap B)$$
$$Card(\overline{A}) = Card(E) - Card(A)$$


De plus : $$Card(E \times F) = Card(E) \times Card(F)$$
