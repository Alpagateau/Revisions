#calculus 
## Définition
Un **développement généralisé** est une généralisation des [[Développements limités|développements limités]].
Il en existes deux sortes :
- Les développements limités généralisés
- Les développements asymptotiques

## Développements limités généralisées
Ce sont des extensions des DL sur les [[Fractions rationnelles]]. On as alors une forme suivante :
$$
f(x) =_0 {b_k \over x^k} +...+ {b_2 \over x^2} + {b_1 \over x} + a_0 + a_1x + a_2 x^2...x^n + o(x^n) 
$$
avec $b_i$ et $a_i$ des réels. 

## Développements asymptotiques
C'est une extension des développements limités qui permettent d'étudier les fonctions au voisinage de $+\infty$. On as alors une forme suivante :
$$
f(x) =_0 {b_k  x^k} +...+ {b_2  x^2} + {b_1  x} + a_0 + {a_1\over x} + {a_2 \over x^2}...{a_n\over x^n} + o({1 \over x^n}) 
$$
Dans la pratique, on se ramène a un DL généralisé en considérant $1\over x$.

## Etude des branches infinies
On appel branche infinie la partie d'une courbe représentative qui tend vers l'infinie en l'infinie. 
On distingue alors trois cas :
1. **Branche parabolique horizontale** : $\lim_{x \to +\infty} {f(x)\over x} = 0$ (c'est le cas de $ln$)
2. **Branche parabolique verticale** :  $\lim_{x \to +\infty} {f(x)\over x} = \infty$ (c'est le cas de $exp$)
3. **Branche oblique** : $\lim_{x \to +\infty} {f(x)\over x} = a, a \in \mathbb{R}$
	-  **Branche parabolique oblique** de direction $y=xa$ : $\lim_{x \to + \infty} f(x) - ax = \infty$ 
	- **Asymptote oblique** d'équation $y = xa+b$ : $\lim_{x \to + \infty} f(x) - ax = b$ 
