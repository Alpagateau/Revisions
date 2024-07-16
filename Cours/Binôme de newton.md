#algebra 
## Coefficient binomial
Écrie $\binom{n}{k}$, le **coefficient binomial** représentes le nombres de groupement de $k$ elements possibles dans un ensemble de $n$ elements.
Il a comme formule générale $\frac{n!}{k!(n-k!)}$.
Quelques valeurs importants:
- $\binom{n}{n} = \binom{n}{0} = 1$
- $\binom{n}{1} = n$
- $\binom{n}{2} = \frac{n(n-1)}{2}$
- $\binom{n}{n-k} = \binom{n}{k}$
- $\binom{n+1}{k+1} = \binom{n}{k} + \binom{n}{k+1}$

![[triangle_de_pascal.png|triangle de pascal]]
## Formule du binôme de Newton
Soient $(a,b) \in \mathbb{C}^2$  
$$
(a+b)^n = \displaystyle \sum_{k=0}^n \binom{n}{k}a^k b^{n-k}
$$
