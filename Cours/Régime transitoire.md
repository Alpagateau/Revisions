#physics
## Définition
Un **régime transitoire** est le passage d'un régime permanent a un autre. Celui-ci se retrouve donc autant dans la mécanique que dans l'électronique.
Un tel régime est souvent décrit par une [[Equations différentielles linéaires#Equation différentielle du premier ordre|équation différentielle d'ordre 1]].

## Cas général
On va considérer ici un circuit électrique RC comme démonstration. Bien entendu, les concepts et techniques utilisées peuvent être transposées sur d'autres régimes transitoires.

![[RC-Circuit.png]]

On considère que $V_e$ est une fonction de $t$ tel que $V_e = \mu \mathcal{U}$[^1] . Ainsi, 
$$
\displaystyle
V_e(t) = 
\left\{ 
\begin{array}{c}
0 \quad , t<0  \\
\mu \quad , t\ge 0 \\
\end{array}
\right. 
$$
On alors cherche l’expression de $V_s$.
>On se concentre ici sur le régime transitoire, donc la résolution de l'équation différentielle est un exercice pour le lecteur. 

On trouve une solution de la forme :
$$
\displaystyle
V_s = \lambda(1-e^{\frac{-t }{ \tau}})
$$
De la on tiens plusieurs choses. 
Premièrement, la limite de $V_s$ en temps infini est $\lambda$.
La forme d'une telle fonction est caractéristique. 
![[Pasted image 20240803181444.png|400]]
Enfin, si on considère deux droites : $y = \lambda$ et $y = V_s'(0)t$, on trouve que ces deux droites se croisent en $t = \tau$. C'est une méthode utile pour trouver certaines valeurs dans un circuit.   



[^1]: $\mathcal{U}$ est appelé **échelon unité** et est utilisé principalement dans la [[Transformée de Laplace]]. 
