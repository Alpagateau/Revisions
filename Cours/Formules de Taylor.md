#calculus 
Les formules de Taylor sont des généralisations du [[Théorème des accroissements finis|théorème des accroissements finis]]. 

## I - Taylor-Lagrange
Soit $f$ une fonction [[Dérivée|dérivable]] $n$ fois, entre $x$ et $x_0$, il existe $c$ tel que :
$$
\begin{align}
f(x) = f(x_0) + (x-x_0)f'(x_0) &+ {(x-x_0)^2 \over 2!}f''(x_0) \\&+\quad... \\&+
{(x-x_0)^{n-1} \over (n-1)!}f^{(n-1)}(x_0) \\&+ 
{(x-x_0)^{n} \over (n-1)!}f^{(n)}(c)
\end{align}
$$
On remarque que, avec $n$ qui augmente, le dernier terme tend vers $0$. 

## II - Taylor-Young
Soit la même fonction $f$ dérivable $n$ fois entre $x$ et $x_0$, on a alors :
$$
\begin{align}
f(x) = f(x_0) + (x-x_0)f'(x_0) &+ {(x-x_0)^2 \over 2!}f''(x_0) \\&+\quad... \\&+
{(x-x_0)^{n} \over (n-1)!}f^{(n)}(x_0) \\&+ 
o_{x_0}(x^n)
\end{align}
$$
Avec ici le terme $o_{x_0}(x^n)$ une fonction inconnue [[Comparaisons locale de fonctions#Fonction négligeable|négligeable]] devant $x^n$. C'est ce genre de formule qui sera utilisée dans le chapitre des [[Développements limités]] 