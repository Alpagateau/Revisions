$P = 1 + 2x - 3x^2 + x^3$
$Q = - 2x + 5x^2 + x^4$  

## Basic idea
1. Turn both into point representation ((degree + 1) points)
2. use symmetry and complex numbers to generate new points
3. multiply
4. interpolate 
## Let's try
$$
\begin{align}
P &= (1 - 3x^2) + (2x + x^3) \\
Q &= (5x^2 + x^4) + (-2x) \\
\end{align}
$$
then 
$$
\begin{align}
P &= A(x^2) + xB(x^2) \\
Q &= C(x^2) + xD(x^2) \\
\text{with} \\
A &= 1 - 3X \\
B &= 2 + X \\
C &= 5X + X^2 \\
D &= -2 \\
\end{align}
$$
$D$ is constant, so trivial to create new points. 
Because $A,B,C,D$ are fonctions of $x^2$, we can use the symmetry to trivially have two values, thus doubling the number of points. 
We can iterate further. Giving :
$$
\begin{align}
A &= (-1) + x(-3) \\
B &= (2) + x(1) \\
C &= (x^2) + x(5) \\
\end{align}
$$
Because Q is of degree 4 and P is of degree 3, we have a maximum degree of 12. We thus need at least 12 values. We consider the 16th root of unity. 
$$
\begin{align}
P(1) &= A(1) + 1 B(1) \\
&= -1-3 + 2 + 1 \\
&= -1 \\

P(e^{2\pi i \over 16}) 
&= A((e^{2\pi i \over 16})^2) + e^{2\pi i \over 16} B((e^{2\pi i \over 16})^2) \\
&= A(e^{2\pi i \over 8}) + e^{2\pi i \over 16} B(e^{2\pi i \over 8}) \\
\end{align}
$$