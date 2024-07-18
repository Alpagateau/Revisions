#arithmetic 
## Division euclidienne
Soit $A, B$ deux [[Polynomes]]
On dit que $B$ divise $A$ ($B \mid A$)
$$
\exists Q \in \mathbb{K}[X], A = B \times Q
$$
On a alors $deg(B) \le deg(A)$. 
En règle générale on défini la division euclidienne de polynômes tel que :
$$
A,B \in \mathbb{K}[X], \exists! (Q, R), \{A= BQ +R, deg(R) < deg(B)\}
$$
On appel **irréductible** un polynôme qui n'admet qu'exactement deux diviseurs unitaires.
- Dans $\mathbb{R}[X]$, tout polynômes de $deg(P) = 1$ ou $deg(P) = 2, \Delta < 0$ est irréductible
- Dans $\mathbb{C}$, seuls les polynômes de $deg(P) = 1$ sont irréductibles. 
On appel **associés** deux polynômes tel que $A \mid B$ et $B \mid A$. Il existe alors un réel $\lambda$ tel que $B = \lambda A$.

## Racines
on appel $a$ une **racine** de $P$ si:
$$
\tilde P(a) = 0 \Leftrightarrow \exists Q, P=(X-a)Q
$$
On dit qu'une racine est de **multiplicité** $m$ (ou **ordre**) si
$$
\exists Q, P = (X-a)^m Q, Q(a) \ne 0
$$
Dans les faits, une racine est de multiplicité $m$ si $P^{(0 \to m-1)}(a) = 0, P^{(m)}(a) \ne 0$.
De la on obtiens que, soit un polynôme a $n$ racines (donc $deg(P) \ge n$) qu'on note $a_i$ avec $i \in [\![1, n]\!]$, on peut donc factoriser $P$.
$$
\displaystyle
\begin{align}
P &= (\prod_{i=0}^n (X-a_i)^{m_i}) \times Q \\
&= Q \times (X-a_1)^{m_1} (X-a_2)^{m_2}(X-a_3)^{m_3}... 
\end{align}
$$
> Si $\mathbb{K} = \mathbb{C}$ et $a$ est une racine, alors $\overline a$ l'est aussi. 

On dit que $P$ est **scindé** si il peut s’écrire comme précédemment avec $Q \in \mathbb{K}$. 
> Tout polynôme non constant sur $\mathbb{C}$ est **scindé**

## Relations coefficients-racines
Soit $P = aX^2 + bX +c$, il existe $(\alpha_1, \alpha_2) \in \mathbb{R}^2$ tel que:
$$
P = a(X - \alpha_1)(X-\alpha_2)
$$
On a alors a relation suivante :
$$
\displaystyle
\left\{ 
\begin{array}{c}
\alpha_1 + \alpha_2 = \frac{-b}{a} \\
\alpha_1 \alpha_2 = \frac{c}{a}
\end{array}
\right. 
$$

 