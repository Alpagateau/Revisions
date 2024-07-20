#calculus
## Définitions
On défini le **taux d'accroissement** de $f$ en $a$, noté $\tau_a$, la fonction sur $D \backslash \{a\}$ tel que 
$\tau_a (x) = \frac{f(x) - f(a)}{x-a}$ 

On dit que $f$ est **dérivable** si $\tau_a$ admet une limite finie en $a$.
Si $f$ est dérivable sur un interval, alors on défini la **dérivé** de $f$, noté $f'$ ou $\frac{df}{dx}$. Si $f$ est derivable, alors $f$ est continue. **Ce n'est pas réciproque**. 
Les dérivées sont stables par combinaisons linéaires. 
## Dérivée usuelles

| Fonction         | Dérivée                    | Domaine                                                                   |
| ---------------- | -------------------------- | ------------------------------------------------------------------------- |
| $x^\alpha$       | $\alpha x^{\alpha -1}$     | $]0, +\infty[$                                                            |
| $e^x$            | $e^x$                      | $\mathbb{R}$                                                              |
| $ln(\mid x\mid)$ | $\frac{1}{x}$              | $\mathbb{R}^*$                                                            |
| $cos(x)$         | $-sin(x)$                  | $\mathbb{R}$                                                              |
| $sin(x)$         | $cos(x)$                   | $\mathbb{R}$                                                              |
| $tan(x)$         | $\frac{1}{cos^2(x)}$       | $\mathbb{R} \backslash \{ \frac{\pi}{2} + k \pi \mid k \in \mathbb{Z} \}$ |
| $ch(x)$          | $sh(x)$                    | $\mathbb{R}$                                                              |
| $sh(x)$          | $ch(x)$                    | $\mathbb{R}$                                                              |
| $th(x)$          | $\frac{1}{ch^2(x)}$        | $\mathbb{R}$                                                              |
| $Arcsin(x)$      | $\frac{1}{\sqrt{1 - x^2}}$ | $]-1, 1[$                                                                 |
| $Arccos(x)$      | $-\frac{1}{\sqrt{1-x^2}}$  | $]-1, 1[$                                                                 |
| $Arctan(x)$      | $\frac{1}{1+x^2}$          | $\mathbb{R}$                                                              |

^2a0507

^du
## Operations entre dérivés

| Fonction         | Dérivée                    | Domaine                |
| ---------------- | -------------------------- | ---------------------- |
| $u^a$            | $a \cdot u' \cdot u^{a-1}$ | dépend de $a$          |
| $\frac{1}{u}$    | $-\frac{u'}{u^2}$          | Si $u$ ne s'annule pas |
| $ln \mid u \mid$ | $\frac{u'}{u}$             | si $u$ n s'annule pas  |
| $e^u$            | $u' \cdot e^u$             |                        |
| $cos(u)$         | $-u' \cdot sin(u)$         |                        |
| $sin(u)$         | $u' \cdot cos(u)$          |                        |
| $tan(u)$         | $\frac{u'}{cos^2(u)}$      |                        |
| $u \cdot v$      | $u'v + uv'$                |                        |
| $\frac{u}{v}$    | $\frac{u'v + uv'}{v^2}$    |                        |
| $u \circ v$      | $v' \times (u' \circ v)$   |                        |
| $u^{-1}$         | $\frac{1}{f'(f^{-1})}$     |                        |
## Dérivés successives
On note $f''$ la seconde dérivée de $f$, puis, de manière plus générale, $f^{(n)}$ est la dérivée $n$-ième de $f$. 
Si une fonction est dérivable $n$ fois, alors sa dérivée $(n-1)$-ième est continue, et toutes ses dérivées jusqu'à $(n-1)$ sont continues. 

## Formule de Leibniz
Soit $f$ et $g$ deux fonctions. On cherche a calculer la dérivée $n$-ième du produit de $f$ et $g$. On peut alors appliquer la **formule de Leibniz** qui est similaire a celle du [[Binôme de newton]]. En effet :
$$
\displaystyle
(f \times g)^n(x) = \sum_{k=0}^n \binom{n}{k}f^{(k)}(x)g^{(n-k)}(x)
$$

