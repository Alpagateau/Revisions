#algebra 
## Définition
On appel **fraction rationnelle** l'équivalent de la division chez les [[Polynomes|polynômes]]. Celle si ce note ainsi :
$$
(P, Q) \in \mathbb{K}[X]^2,\quad Q \ne 0,\quad F = {P \over Q}
$$
On note $\mathbb{K}(X)$ l'ensemble des fractions rationnelles.

## Points communs avec les fractions
Tous comme les rationnels, on définit l'équivalence des fractions rationnelles comme suit :
$$
{P \over Q} = {E \over F} \Leftrightarrow P \cdot F = E \cdot Q
$$
>Si $F = {P \over Q}$ et $P$ et $Q$ sont premiers entre eux, on dit que $P \over Q$ est **un** représentant irréductible de $F$. Il n'existe qu'un seul tel couple $(P, Q)$ a une multiplicative près.

**Les opérations entre fractions rationnelles sont les mêmes qu'avec les fractions simple**. 
Par exemple :
$$
\begin{align}
{P_1 \over Q_1} + {P_2 \over Q_2} &= {P_1Q_2 + P_2Q_1 \over Q_1 Q_2} \\
{P_1 \over Q_1} \times {P_2 \over Q_2} &= {P_1 P_2 \over Q_1 Q_2}
\end{align}
$$

## Composition, conjugué et degré
Les fractions rationnels sont stable par composition. En l'occurrence, on définit :
$$
F \circ G = {P \circ G \over Q \circ G}
$$
De même, si la fraction est dans $\mathbb{C}(X)$, on définit aussi le conjugué.
$$
\overline F  = {\overline P \over \overline Q}
$$
Enfin on définit le [[Polynomes#Degré|degré]] de $F$ en fonction de $P$ et de $Q$, en effet :
$$
deg(F) = deg(P) - deg(Q)
$$
C'est en quelque sorte l'inverse de la multiplication polynomiale. 
Les propriétés des opérations entre les degrés sont les mêmes que pour les polynômes. 

## Zéros et pôles
On appels **zéros** d'une fractions rationnels les points en lesquels celle-ci s'annule, ce qui équivaut aux points pout lesquels $P$ s'annule. On voit encore ici un parallèle avec les fractions. En effet, un si son numérateur vaux zéros, alors la fraction entière vaux zéros. 
Un **pôle** est un point pour lequel le dénominateur s'annule. Pour le visualiser, on imagine une fonction de la forme $\frac{1}{x}$. Quand $x$ tend vers zéros, la fraction tends vers l'infini. C'est ça un pôle. Une fraction rationnelle n'est pas défini sur les pôles. 
Les zéros et les pôles de $F$ sont donc les [[Calcul Polynomial#Racines|racines]] de $P$ et $Q$. 
On a alors la même idée de **multiplicité** que ce soit pour les pôles ou les zéros.
