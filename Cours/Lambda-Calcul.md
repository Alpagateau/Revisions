#calculus 
## Définition
Le **lambda-calcul** ou $\lambda$-calcul a été inventé par Alonzo Church, maître de thèse d'Alan Turing. La théorie de Church-Turing affirme que le $\lambda$-calcul est équivalent a une Machine de Turing, d'un point de vue mathématique. 
Selon le $\lambda$-calcul, une [[Fonctions de la variable réelle|fonction]] est une boite noire, qui accepte une (ou plusieurs) entrée, la considère et produit une sortie. Il est impossible de voir ce qu'il se passe a l’intérieur des fonctions. Elles sont considéré comme "magique", dans le sens où aucun effet secondaire, ni aucune information autre que les entrées ne sont possibles. 

## Syntaxe
$$
\begin{align}
\lambda x.x+1 & \rightarrow f(x) = x+1 \\
\lambda x . \lambda y . x+y & \rightarrow f(x,y) = x+y

\end{align}
$$
## Encodage
Ceci est un encodage couramment utilisé:
$$
\begin{align}
V & \rightarrow \lambda x.\lambda y. x  \\
F & \rightarrow \lambda x.\lambda y. y \\
Not &: \lambda b . b \space F \space V \\
\end{align}
$$
