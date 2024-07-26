#calculus 
## Définition
Une **équation différentielle** est tout simplement une équation qui met en relation une [[Fonctions de la variable réelle|fonction]] et ses [[Dérivée|dérivées]]. Celles-ci sont très utiles pour modéliser une grande partie des phénomènes physiques. 
Il existes deux sortes d'équations différentielles : 
- Les équations différentielles ordinaires (ODE), pour lesquels les fonctions étudiées sont a une variables
- Les équations différentielles partielles (PDE), pour les fonctions a plusieurs variables.
Ici nous n'étudierons que les fonctions a une seule variable.

## Notation
Une équation différentielle du premier ordre (nous allons voir ce que cela veux dire juste après) aura la forme suivante :
$$
(E)\quad\quad y' + a(x)y = b(x)
$$
avec $a$, $b$ et $y$ des fonctions. 

## Notion d'ordre
On appel l'ordre d'une équation différentielle le nombre maximum de dérivées de $y$ nécessaire. Cette notion est similaire a la notion d'ordre pour les [[Polynomes|polynomes]].
Plus l'ordre d'une equa-diff est grand, plus celle-ci est difficile a résoudre. Ici, nous verrons les ordre 1 et 2.
Pour les ordres trop grands, nous ne serons pas capable de trouver une solution analytique, et devrons donc trouver des solutions numériques en utilisant des solutions [[Intégration discrète|discrètes]]. 

## Equation différentielle du premier ordre
Comme dit précédemment, une équation différentielle du premier ordre s'écrirait ainsi :
$$
(E) \quad \quad y' + a(x)y = b(x)
$$
Résoudre une telle équation, c'est trouver toutes les fonctions $y$ qui vérifies l'équation $E$. Pour cela, on va se servir de la linéarité de ces équations.
On va alors considérer deux fonctions particulières :
- $y_H$ la solution a l'équation **homogène** : $(H) \quad y' + a(x)y = 0$
- $y_p$ une solution particulière de $E$, plus facile a trouver
On découpe ce problème en deux, car la solution générale d'une telle équation est simplement la somme de $y_H$ et $y_p$.
### Solution homogène
On cherche donc $y_H$ tel que :
$$
\begin{align}
y_H' + a(x)y_H & = 0 \\
y_H' &= -a(x)y_H
\end{align}
$$
On se rappelle alors, dans le chapitre des [[Dérivée]], que pour $u$ une fonction dérivable:
$$
(e^u)' = u'\cdot e^u
$$
On remarque par identification que $y_H = e^u$ et que $u' = -a(x)$.
Pour trouver $u$, on intègre alors $a(x)$ et on obtient une forme générale pour la solution homogène :
$$
y_H = \lambda e^{-A(x)}, \quad \lambda \in \mathbb{R}, \quad A'(x) = a(x)
$$
On a trouvé la solution homogène. 
>Attention, ici on ne cherche pas a déterminer $\lambda$, cela ce fait via les conditions initiales, mais on appel cela un **problème de Cauchy**.
### Solution particulière
La deuxième partie de la résolution d'une telle équation passe par la recherche d'une solution particulière, quelle qu'elle soit. 
Il existe différentes méthodes pour trouver une telle solution.
##### Tout simplement deviner
Il suffit ici de trouver une seule fonction qui vérifie l'équation. On a tout a fait le droit de juste deviner une solution. Cela peut s'avérer utile sur les fonctions connus comme $cos$, $sin$.....
##### Si a et b sont multiples l'un de l'autre
Si il existe un $\lambda$ tel que pour tout $x$, $\lambda a(x) =b(x)$, alors, on considère que $y$ est une fonction constante. 
On a alors le résultat suivant :
$$
\begin{align}
y_p &= \lambda, \quad \lambda \in \mathbb{R} \\
y_p' &= 0 \\
a(x)\lambda &= b(x)
\end{align}
$$
$y_p$ est donc solution. 
Hélas, cette méthode est très simple, mais fonctionne rarement. 
##### Méthode de variation de la constante
C'est la méthode la plus robuste, mais aussi la plus complexe pour trouver la solution particulière. 
On suppose que $y_p$ est une solution et que celle ci est de la forme :
$$
y_p = g(x)e^{-A(x)},\quad A' = a
$$
Il ne reste alors qu'a trouver la fonction $g$ pour avoir $y_p$. Pour cela, on sait, par supposition, que $y_p$ vérifie l'équation, on la réinjecte donc.
$$
\begin{align}
y_p' + a(x)y_p &= b(x) \\
(g(x)e^{-A(x)})' + a(x)\cdot g(x)e^{-A(x)} &= b(x) \\
g'(x)e^{-A(x)}-g(x)a(x)e^{-A(x)} + g(x)a(x)e^{-A(x)} &= b(x) \\
g'(x)e^{-A(x)} &= b(x) \\
g'(x) &= {b(x)\over e^{-A(x)}} \\
g'(x) &= {b(x)\cdot e^{A(x)}} \\
\end{align}
$$
On intègre alors le second membre, et on obtient $g$. 
On a trouvé une solution particulière !
##### Principe de superposition
Si il existe $b_1, b_2$ tel que $b = b_1 + b_2$, alors on peut trouver une solution particulière pour $b_1$ puis $b_2$ et les additionner pour obtenir $y_p$.
##### Cas particuliers
1. Si $a$ est une constante et $b$ est de la forme $P(x)e^{sx}$ avec $P$ un polynôme et $s$ un réel, on a alors :
$$
y_p :x \rightarrow 
\begin{dcases}
    Q(x)e^{sx},& s \ne a \\
    xQ(x)e^{sx}, & s = a
\end{dcases}
$$
	avec $Q$ un polynôme de même degré que $P$. 
2. Si $a$ est une constante et $b$ est de la forme $b \rightarrow \lambda cos(\omega x) + \mu sin(\omega x)$, alors :
$$
y_p = \alpha cos(\omega x) + \beta sin(\omega x)
$$

## Equations différentielles du second ordre
> Ici nous n'étudieront que les equa-diff d'ordre 2 **a coefficients** constants.

Une équation du second ordre serait alors de cette forme :
$$
(E) \quad ay'' + by' +cy = f(x)
$$
avec $(a,b,c) \in \mathbb{R}^3$.
La méthode de résolution est similaire. On essaie d'abord de résoudre l'équation homogène, puis on l'additionne a une solution particulière. 
##### Solution homogène 2nd ordre
La solution homogène est un peu plus complexe a trouver pour l'ordre deux. On commence par considérer le **polynôme caractéristique** de l'équation :
$$
(E_c)\quad ar^2 + br + c = 0, \quad r\in \mathbb{C}
$$
On a alors trois cas. Soit :
- il existes deux racines réelles $r_1, r_2$ alors on a :
$$
y_H = \lambda e^{r_1 x} + \mu e^{r_2 x}
$$
- Il existes une racine double réelle $r$, ainsi:
$$
y_H = (\lambda x + \mu)e^{rx}
$$
- Il existes deux racines [[Nombres complexes|complexes]] $\alpha \pm i \beta$ :
$$
y_H = e^{\alpha x} (\lambda cos(\beta x) + \mu sin(\beta x))
$$
> Le pourquoi du comment est un peu long mais est très bien expliqué sur le site de [Paul's Online Notes](https://tutorial.math.lamar.edu/classes/de/complexroots.aspx).

##### Recherche d'une solution particulière 2nd ordre
La recherche de solution particulière pour le 2nd ordre est plus complexe que pour le premier ordre. Ici sont présentés quelques cas particuliers 

1. $f(x)$ est de la forme $P(x)e^{rx}$ avec $P$ un polynôme non constant et $r \in \mathbb{C}$. Alors on a :
$$
y_p : x \rightarrow
\begin{dcases}
Q(x)e^{rx}&,  r\text{ n'est pas racine de } E_c \\
xQ(x)e^{rx}&,  r \text{ est racine simple de } E_c \\
x^2Q(x)e^{rx}&, r\text { est racone double de } E_c
\end{dcases}
$$
2. $f(x)$ est de la forme $P(x)cos(\omega x)$ (resp. $sin$), on applique la méthode précédente en considérant $f_2(x) = P(x) e^{i \omega x}$ . Puis on prend la partie réelle de la solution (resp. la partie imaginaire pour $sin$).