## Définition
Le régime **pseudo périodique** est un régime particulier d'un [[Oscillateur Harmonique#OH amortie|oscillateur harmonique amortie]] pour lequel le facteur qualité $Q$ est supérieur a $1 \over 2$. 
Ce régime correspond a un amortissement plus faible que la force d'oscillation. 

On rappel :
$$
\ddot x + {\omega_0 \over Q} \dot x + \omega_0^2 x = 0
$$
Le polynôme caractéristique est donc :
$$
 r^2 + {\omega_0 \over Q} r + \omega_0^2 = 0
$$
On sait que le polynôme accepte deux solutions, car le $Q > {1\over 2}$. On note ces solutions complexes $r_1$ et $r_2$.
Ainsi :
$$
r_{12} = -{\omega_0 \over 2Q} \pm i \omega_0 \sqrt{ 1 - {1 \over4Q^2} }
$$
On pose alors deux variables :
$$
\begin{align}
\alpha &= {\omega_0 \over 2Q} \\
\omega &= \omega_0 \sqrt{1 - {1 \over 4Q^2}}
\end{align}
$$
Ainsi, on obtient :
$$
x(t) = Ae^{-\alpha t} cos(\omega t + \phi)
$$
On observe alors deux parties :
- La partie oscillation, avec la fonction cos
- La partie amortissement, qui correspond a un [[Régime transitoire]].
