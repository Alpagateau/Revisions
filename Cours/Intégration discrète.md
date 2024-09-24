#calculus 
L'intégration discrete, ou numérique, est une technique d'approximation numérique des solutions d'[[Equations différentielles linéaires|equations différentielles]]. Il existe différentes méthodes. Dans ce document, $h$ est le pas. 

## Méthode d'Euler
C'est la méthode la plus simple d'intégration numérique. Elle nécessite $t_0,\space y(t_0)$ et $y'(t, y(t))$. De la, c'est une méthode itérative. Voici la méthode :
On pose que $y'(t_0) \approx \frac{y(t+h) - y(t)}{h}$. On obtiens donc, par récursion les relations suivantes : 
1. $y_1 = y_0 + h \times y'(t_0, y_0)$
2. $y_2 = y_1 + h \times y'(t_0 + h, y_1)$
3. $y_3 = ....$

## Méthode inverse d'Euler
Cette méthode est un peu plus complexe car nécessite la résolution d'une équation pour obtenir $y_{n+1}$. On l'appel méthode inverse car on approxime la dérivée a gauche, au lieu d'a droite. On considère donc $y'(t) \approx \frac{y(t) - y(t-h)}{h}$, de la on tire la relation suivante :
$$
y_{n+1} = y_n + hf(t_{n+1}, y_{n+1})
$$
Il faut alors résoudre pour $y_{n+1}$. Des méthodes comme la **méthode de Newton** peuvent être utilisées. Cette méthode est souvent plus stable que la méthode directe, mais plus lourde en calcul. 

## Méthode Runge-Kutta
[Video sur RK4](https://www.youtube.com/watch?v=dShtlMl69kY)
Soit les valeurs de départ suivantes :
$$
y' = f(t, y), \quad y(t_0) = y_0
$$
L'algorithme est donc comme suit :
$$
\begin{align}
y_{n+1} & = y_n + \frac{h}{6}(k_1 + 2k_2 + 2k_3 + k4) \\
k_1 & = f(t_n, y_n) \\
k_2 &= f(t_n + \frac{h}{2}, y_n+h \frac{k_1}{2}) \\
k_3 &= f(t_n + \frac{h}{2}, y_n+h \frac{k_2}{2}) \\
k_4 &= f(t_n + h, y_n + h k_3)
\end{align}
$$
Cette méthode est plus lourde que la méthode d'Euler, mais est aussi beaucoup plus précise et stable. La généralisation de cette méthode donne la relation suivante :
$$
\begin{align}
y_{n+1} &= y_n + h \sum_{i=1}^s b_i k_i
\end{align}
$$
où
$$
\begin{align}
k_i &= f(t_n + c_i, y_n + \sum_{j=1}^{i-1} a_{ij}k_j)
\end{align}
$$
Pour calculer $a$, $b$ et $c$, voir [Runge-Kutta](https://en.wikipedia.org/wiki/Runge%E2%80%93Kutta_methods). 
## Intégration exponentielle de premier ordre
Ici, on suppose que l'equation est de la forme suivante : 
Soit $A$ un scalaire et $N(y)$ un terme non-linéaire :
$$
y'(t)=-Ay + N(y) 
$$
Pour intégrer, on considère $N(y)$ constant sur un interval $h$. On obtiens alors, par intégration : 
$$
\displaystyle
y_{n+1} = e^{-Ah} + A^{-1}(1-e^{-Ah}) N(y(t_n))
$$

