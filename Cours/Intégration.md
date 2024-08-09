#calculus 
## Définition
L'**intégrale** d'une fonction $f$ est l'air algébrique sous la courbe entre deux bornes.
![[Pasted image 20240710225930.png]]
Les intégrales sont linéaires et respectent la relation de Chasles.  
On appel la fonction qui, une fois dérivée donne $f$, la primitive de $f$.
On ne peut intégrer que les fonctions continues par morceaux.  
>Cette page explique l'intégration [[Continuité|continue]], pour l'intégration discrète voir cette [[Intégration discrète|page]].
##### Théorème fondamental de l'analyse
$$
F(x) = \displaystyle \int_{a}^{b} f(x)\,dx
$$
## Calcul d'une intégrale
$$
\displaystyle \int_{a}^{b} f(x)\,dx = [F(x)]_a^b = F(b) - F(a)
$$
Pour la majorité des intégrales usuelles, il faut juste lire les [[Dérivée#^2a0507|dérivées usuelles]].

## Intégration par parties
$$
\displaystyle \int_a^b u'(x)v(x)\,dx = [u(x)v(x)]_a^b - \int_a^b u(x)v'(x), dx
$$
## Intégrations multiples
Pour intégrer plusieurs fois,  on les considères imbriqués.
Par exemple :
$$
\displaystyle V = \int_0^a \int_0^b \int_0^c (x+z) \times y\, dzdydx
$$
Pour calculer cela, on commence par $z$. On considère $x$ et $y$ constantes, et on intègre. 
$$
\displaystyle V_z = \int_0^c (x+z) y\, dz = y[zx+\frac{1}{2}z^2]_0^c = y(cx + \frac{1}{2}c^2)
$$
donc,
$$
\displaystyle V = \int_0^a \int_0^b y(cx + \frac{1}{2}c^2)\, dydx
$$
Ensuite, on intègre sur $y$
$$
\displaystyle V = \int_0^a  \frac{1}{2}b^2(cx + \frac{1}{2}c^2)\, dx
$$
Puis sur $x$
$$
\displaystyle V =  \frac{1}{2}b^2(ca^2 + \frac{1}{2}c^2a)
$$
