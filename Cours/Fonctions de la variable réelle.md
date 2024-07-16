#calculus
## Définition
Une fonction (ou application) de $\mathbb{R}$ et $\mathbb{R}$ est une "boite" qui a chaque réel associe un autre réel. 

Soit une fonction $f$,
- $f$ est **injective** si toute image admet **au plus un antécédent**
$$
\forall (x_1, x_2) \in A^2, f(x_1) = f(x_2) \Rightarrow x_1 = x_2
$$
- $f$ est **surjective** si toute image admet un antécédent.
$$
\forall y, \exists x, f(x)= y
$$
- $f$ est **bijective** si elle est injective et surjective. Il existe alors $f^{-1}$ la réciproque. ^bd2e7f

## Majoration
On dit que $f$ est majorée sur $A$ si
$$
\exists M \in \mathbb{R}, \forall x \in A, f(x) \le M
$$
de meme pour minorée.
$f$ est bornée si $A$ est majorée et minorée. On peut aussi borner une fonction par la valeur absolue, ainsi :
$$
\exists M \in \mathbb{R}^+, \forall x \in A, |f(x)| \le M
$$
Une fonction bornée n'admet pas forcements d'extremums, mais si elle en admet, alors :
$$
\exists \alpha, \forall x \in A, f(x) \le f(\alpha)
$$
## Operations usuelles
$$
(f+g)(x) = f(x)+g(x)
$$
$$
(f \cdot g) = f(x) \cdot g(x)
$$
$$
k\in \mathbb{R}, \quad (kf)(x) = k \cdot f(x) 
$$
$$
(f \circ g) = f(g(x))
$$
## Parité et périodicité
- une fonction est dite **paire** si $f(x) = f(-x)$
- une fonction est **impaire** si $f(x) = -f(-x)$
- une fonction est **périodique** si $$\exists T \in \mathbb{R}_+^*, \quad \forall x \in \mathbb{R}, \quad f(x+T) = f(x) $$
## Monotonie

1. **croissant** : $\forall (a,b) \in A^2, a \le b \Rightarrow f(a) \le f(b)$ (resp. strictement)
2. **décroissante** : $\forall (a,b) \in A^2, a \le b \Rightarrow f(a) \ge f(b)$ (resp. strictement)

Soient $f$ et $g$ monotones, $f \circ g$ est monotone. 
Si $f$ est strictement monotone, alors $f$ est bijective et $f^{-1}$ a le meme sens de monotonie que $f$. 

## Continuité
Une fonction est dite continue si, pour tout $x_0$, $\displaystyle \lim_{x\to x_0} f(x) = f(x_0)$  
La continuité est conservé par les operations usuelles. 

## Dérivée et intégrale
Par souci de clarté, les articles sur les [[Dérivée|dérivées]] et [[Intégration|intégrales]] sont dans des pages séparées.
## Quelques fonctions utiles
- [[Fonctions trigonométriques]]
- logarithme népérien : $ln(x)$
- logarithme : $ln_a(x) = \frac{ln(x)}{ln(a)}$
- [[Fonctions hyperboliques]]