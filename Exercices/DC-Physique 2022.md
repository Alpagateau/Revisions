# Partie 1
## A) Comportement mécanique du système 
On étudie une dalle qui récupère l'énergie de dancers pour en faire de l'électricité. On modélise cette dalle par une plaque carrée de 65 cm de coté, et de masse = 35 kg. 
On considère qu'elle reste constamment horizontale.
Elle est repéré par sa position $z(t)$ sur l'axe vertical. On note $v(t) = \dot z(t) \vec{e_z}$. On a $g = 10m.s^{-2}$ la gravité. 
La dalle est reliée a un ressort de longueur a vide $l_0$ et de raideur $k$, ainsi qu'un amortisseur mécanique. 

On a alors 4 forces :
- $\vec{P} = -mg\vec{e_z}$ 
- $\vec{F_r} = -k(l_0 - z(t))\vec{e_z}$ 
- $\vec{F_{\lambda}} = -\lambda\vec{v}, \lambda > 0$
- $\vec{F_{\alpha}} = -\alpha \vec{v}, \alpha > 0$
### 1 : Exprimer la force du ressort
$$
\vec{F_r} = -k(z(t) - l_0)\vec{e_z}
$$
### 2 : Determiner la position d'équilibre de la dalle a vide
$$
\begin{align}
\text{Par definition on a que }: \\
-mg &= k(z_{eq} - l_0) \\
-{mg \over k} &= z_{eq} -l_0 \\
z_{eq} &= -{mg \over k} + l_0
\end{align}
$$
### 3: Position a l'équilibre avec un danseur
Un danseur de masse $M$ monte sur la dalle. 
On a alors 
$$
z_{eq}' = {(m+M)g \over k} + l_0
$$
On pose l'affaissement:
$$
\begin{align}
\delta &= z_{eq} - z'_{eq} \\
&= {mg \over k} - {(m+M)g \over k} \\
&= { g(m - m - M) \over k} \\
&= -{gM \over k}
\end{align}
$$
### 4 : Trouver une raideur 
On suppose un homme de poids moyen $M = 80kg$. On alors :
$$
\delta = {800 \over k}m \cdot s ^{-2}
$$
On veux que $\delta$ soit limité a quelques millimètres. Ainsi :
$$
\begin{align}
\delta &< 0.005 \\
{800 \over k} &< 0.005 \\
{k \over 800} &> 200 \\
k &> 160k
\end{align}
$$
### 5 : Trouver l'équation différentielle
On pose d'abord $Z(t) = z(t) - z_{eq}$
On utilise alors la seconde lois de Newton
On a alors :
$$
\begin{align}
\ddot z(t)m &= P + F_r + F_{\lambda} + F_{\alpha} \\
\ddot z(t)m &= -mg -k(z(t) - l_0) - \lambda \dot z(t) - \alpha \dot z(t) \\
\ddot z(t)m + (\lambda + \alpha) \dot z(t) +k(z(t) - l_0) &= -mg \\
\ddot Z(t)m + (\lambda + \alpha)\dot Z(t) + k(z(t)-l_0) &= -mg
\end{align}
$$
Si on considère une solution constante a cette équation, on obtiens $z_{eq}$. Par le principe de superposition, on a que $Z(t)$ est une solution, ainsi :
$$
\begin{align}
\ddot Z(t)m + (\lambda+ \alpha)\dot Z(t) + k Z(t) &= 0 \\
\ddot Z(t) + {\lambda+ \alpha \over m} \dot Z(t) + {k\over m }Z(t) &= 0
\end{align}
$$
Ainsi :
$$
\begin{align}
\omega_0 &= \sqrt{{k\over m}} \\
{\omega_0 \over Q} &= {\lambda+ \alpha \over m} \\
{1 \over \omega_0 Q} &= m(\lambda + \alpha) \\
Q &= {\sqrt{km} \over \lambda + \alpha}

\end{align}
$$
> Conditions initiales 
> Lestée d'un masse $M$, la dalle est au repose
> A t=0, on retire cette masse $M$

$$
Z(0) = -\delta
$$
$$
\dot Z(0) = 0
$$
## A.1 Pas de force d'amortissement
On pose m=35 kg et $\alpha = \lambda = 0$. 
$$
{\omega_0 \over Q} = {\omega_0 (\alpha+\lambda) \over \sqrt{km}} 
= 0
$$
### 6: Résolution d'équation
On a l'équation 
$$
\begin{align}
\ddot Z(t) + \omega_0^2Z(t) &= 0 \\
Z(t) &= Acos(\omega_0t + \phi)\\
\phi &= 0 \\
A &= -\delta
\end{align}
$$
### 7: Calculs littéral 
$$
\begin{align}
T &= {\omega_0 \over 2\pi} \\
Z_{min} &= z_{eq} - \delta \\
Z_{max} &= z_{eq} + \delta \\
\end{align}
$$
Application numérique :
$$
\begin{align}
T &= {100 \over 2\pi} \\
\end{align}
$$
## A.2 : Amortissement uniquement mécanique
On a que la masse vaut 35 kg. De plus, on sait que $\omega_0 = 100rad \cdot s^{-1}$. On a donc :
$$
\begin{align}
\omega_0 = 100 = \sqrt{k \over m} = \sqrt{k\over 35} \\
\omega_0^2 = 10000 = {k\over35} \\
k = 350000
\end{align}
$$
### 9 : Equation caractéristique
$$
\begin{align}
r^2 + {\lambda \over m}r + {k\over m} &= 0 \\
\Delta &= ({\lambda\over m})^2-4{k\over m}
\end{align}
$$
A la vue du graph, on peut déduire que le discriminent est négatif. 

### 10 : Trouver Tau
On a que $\tau = {\omega_0 \over 2Q}$ 

### 11 : Vitesse de décroissement
$$
\begin{align}
e^{-t\over \tau} &= 0.5 \\
{-t\over \tau} &= -ln(2) \\
t &= \tau ln(2) \\
\end{align}
$$
### 12 : Determiner Q
$$
t_1 = 1.10 s \rightarrow \tau = 1.586 
\rightarrow {\omega_0 \over 2Q} = 1.586
\rightarrow {1 \over 1.586} = {2Q \over 100}
\rightarrow {100 \over 3.172} = Q 
$$
$$
Q = 31.52
$$ 