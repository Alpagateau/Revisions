#calculus 
## Cercle unitaire définitions
Le **cercle unitaire** est un cercle centré en $(0,0)$ de rayon $1$. La position de chaque point sur ce cercle est défini par $(cos (a), sin (a))$ avec $a \in \mathbb{R}$. On défini la **tangente** de $a$ par $tan(a)=\frac{sin(x)}{cos(x)}$ ^b2d326

![[Pasted image 20240710181517.png]]

Les [[Fonctions de la variable réelle|fonctions]] $sin$ et $cos$ admettent des definitions suivant les [[Nombres complexes|complexes]] :

$$
sin(x) = \frac{e^{ix} - e^{-ix}}{2i} \quad
cos(x) = \frac{e^{ix} + e^{-ix}}{2}
$$
Mais aussi des [[Développements limités|développement limités]] :
$$
sin(x) = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!}...
$$

$$
cos(x) = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \frac{x^6}{6!}...
$$

## Valeurs remarquables

| x               | cos                  | sin                  |
| --------------- | -------------------- | -------------------- |
| $0$             | $1$                  | $0$                  |
| $\frac{\pi}{6}$ | $\frac{\sqrt{3}}{2}$ | $\frac{1}{2}$        |
| $\frac{\pi}{4}$ | $\frac{\sqrt{2}}{2}$ | $\frac{\sqrt{2}}{2}$ |
| $\frac{\pi}{3}$ | $\frac{1}{2}$        | $\frac{\sqrt{3}}{2}$ |
| $\frac{\pi}{2}$ | $0$                  | 1                    |
>Mnémotechnie : Pour sin, on écrit 0 1 2 3 4, on met tout a la racine, et on divise par 2 ^^ 

## Formules importantes
- $cos^2(x) + sin^2(x) =  1$
- $cos(a+b) = cos(a)cos(b) - sin(a)sin(b)$
- $sin(a+b) = sin(a)cos(b) + sin(b)cos(a)$
- $cos(2a) = cos^2(a)-sin^2(a)$
- $sin(2a) = 2sin(a)cos(a)$
- $cos(a)cos(b) = \frac{1}{2} (cos(a+b) + cos(a-b))$
- $sin(a)sin(b) = \frac{1}{2}(cos(a-b)+cos(a+b))$
- $sin(a)cos(b) = \frac{1}{2} (sin(a+b)+sin(a-b))$
- $cos(a)+cos(b) = 2cos(\frac{a+b}{2})cos(\frac{a-b}{2})$
- $cos(a)-cos(b) = -2sin(\frac{a+b}{2})cos(\frac{a-b}{2})$
- $sin(a)+sin(b) = 2sin(\frac{a+b}{2})cos(\frac{a-b}{2})$
- $sin(a)-sin(b) = 2cos(\frac{a+b}{2})sin(\frac{a-b}{2})$

## Fonctions réciproques
Les fonctions trigonométriques sont [[Fonctions de la variable réelle#^bd2e7f|bijéctives]] sur $[-1,1]$. Leurs fonctions réciproques sont donc :
- $Arcsin \rightarrow [-\frac{\pi}{2}, \frac{\pi}{2}]$
- $Arccos \rightarrow [0, \pi]$
La fonction $Arctan$ elle est définie : $Arctan : \mathbb{R} \rightarrow [-1,1]$
Elles sont aussi souvent représentées par leurs fonctions [[Dérivée#^du|dérivées]]

## Linéarisation de cos et sin
##### Formule d'Euler
$$
sin(x) = \frac{e^{ix} - e^{-ix}}{2i} \quad
cos(x) = \frac{e^{ix} + e^{-ix}}{2}
$$
De la on obtiens que  
$$
sin(x)^p = ( \frac{e^{ix} - e^{-ix}}{2i})^p \rightarrow
(2i)^p \cdot sin(x)^p = (e^{ix} - e^{-ix})^p
$$
$$
\displaystyle (e^{ix} +(- e^{-ix}))^p = \sum_{k=0}^p e^{ix + k} (-e^{ix})^{p-k}
$$
Ensuite, on simplifie grace au [[Binôme de newton]]

##### Factorisation par l'angle moitié
Cette méthode permet de factoriser $1 + e^{ia}$ et $e^{ia} - e^{ib}$
$$
\begin{align}
1+e^{ia} = e^{i0} + e^{ia} \\
= e^{i \frac{a}{2}}(e^{-i \frac{a}{2}} + e^{i \frac{a}{2}})
\end{align}
$$
On remarque la formule d'Euler, donc :
$$
=2cos(\frac{a}{2})e^{i \frac{a}{2}}
$$
Maintenant pout le second exemple : 
$$
\begin{align}
e^{ia} - e^{ib} = e^{i\frac{a+b}{2}}(e^{i\frac{a-b}{2}} - e^{i\frac{b-a}{2}}) \\
= e^{i \frac{a+b}{2}} \cdot 2isin(\frac{a-b}{2})
\end{align}
$$