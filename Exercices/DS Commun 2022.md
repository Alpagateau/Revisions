On cherche a étudier certaines propriétés de la fonction $F$ définie par :
$$
\forall x \in \mathbb{R}, F(x) = \int_0^x {sin(t) \over t} dt
$$
On remarque que la fonction $F$ est l'intégrale de la fonction [[sinus cardinal]]. 
## Partie I
On pose $f$ la fonction **sinus cardinal** définie par 
$$
\forall t \in \mathbb{R}^*, f(t)={sin(t) \over t}, f(0)= 1
$$
1. Déterminer un [[Développements limités|développement limité]] a l'ordre 2 en 0 de $f$. 
> **Réponse** :
> On a que $sin(t) =_0 t - {t^3 \over 6} + o(t^3)$ 
> On divise alors par $t$ et on obtiens :
> $f(t) = 1 - {t^2\over 6} + o(t^2)$

2. Justifier que $f$ est [[Continuité|continue]] sur $\mathbb{R}$.
>**Réponse** :
>Par définition, $f$ est continue en 0 ssi $f$ admet une limite finie en 0
>On a :
>  $f = 1 - {t^2 \over 6} + o(t^2)$
>  or
>  $\lim_{t \to 0} t^2 = 0$ 
>  i.e.
>  $\lim_{t \to 0} f(t) = 1 = f(0)$

3. On pose alors $F$ définie ci-haut. Justifier que $F$ est bien définie sur $\mathbb{R}$, puis qu'elle est de classe $\mathcal{C}^1$ sur $\mathbb{R}$. 
>**Réponse** : 
>Une [[Intégration|intégrale]] est définie ssi la fonction a intégrer est continue par morceaux. 
>$f$ est continue sur $\mathbb{R}$ et donc particulièrement continue par morceaux. $F$ est donc bien définie sur $\mathbb{R}$.
>De plus, selon le [[Théorème fondamental de l'analyse]], $F$ étant l'intégrale de $f$, $f$ est la [[Dérivée|dérivée]] de $F$. On a que $f$ est continue donc $F$ est continue car dérivable et sa dérivée est continue donc $F$ est de classe $\mathcal{C}^1$. 

4. Résoudre l'[[Equations différentielles linéaires|équation différentielle]] :
$$
(E) \quad x^2y'+xy= sin(x)
$$
sur $\mathbb{R}^*_+$ et sur $\mathbb{R}^*_-$. 

>**Réponse** :
>On suit simplement la méthode[^1] . On considère d'abords l'équation homogène.
>On considère d'abord $\mathbb{R}_+^*$
>	$(H) \quad x^2y'+xy=0$
>	$(H) \quad y'+{1 \over x}y = 0$
>On a que $ln'(x) = {1\over x}$ , ainsi :
>	$y_h^+ = \lambda e^{-ln(x)} = {\lambda \over x}$
>
>On cherche alors une solution particulière. On utilise la méthode de variation de la constante. 
>On pose une solution particulière $y_p = \lambda(x)e^{-ln(x)} = { \lambda(x) \over x}$ 
>Ainsi :
>	$(E_p) \quad x^2{\lambda'(x)x - \lambda(x) \over x^2} + \lambda(x) = sin(x)$
>	$(E_p) \quad \lambda'(x)x = sin(x)$
>	$(E_p) \quad \lambda'(x) = {sin(x) \over x}$
>	$(E_p) \quad \lambda(x) = F$	
> Donc, $y_p = {F \over x}$
> Ainsi, la solution sur $\mathbb{R}^*_+$ est $y = {F \over x} + {\lambda \over x}$
> On considère maintenant $\mathbb{R}^*_-$.
> On a que $ln'(-x) = {1 \over -x}$  
> 	$y_h^- = \lambda e^{-(-ln(-x))} = {\lambda \over x}$ 
> La suite est identique. 

5. Soit $g$ une solution de $E$ sur $\mathbb{R}^*$, on note $\lambda^+, \lambda^-$ les constantes réelles permettant d'exprimer $g$ en avant et après 0. Quelle condition sur $\lambda^+, \lambda^-$ permet de prolonger $g$ en 0 ?
> **Réponse** :
> On rappel que pour prolonger par continuité, on doit avoir $\lim_{x \to 0^-} g(x) = \lim_{x \to 0^+} g(x)$.
> On a 
> 	$F(x) = \int_0^x f(t)dt \sim_0 \int_0^x 1 - {t^2 \over 6} + o(t^2)dt = x - {t^3 \over 18} + o(t^3)$ 
> 	$\lim_{x \to x \to 0^-} {F(x) \over x} = 1$
> 	Donc 
> 	$\lim_{x \to 0^-} g(x) = \lim_{x \to 0^+} g(x) \Leftrightarrow \lambda^+ = \lambda^- = 0$

6. Montrer que $(E)$ n'admet qu'une solution sur $\mathbb{R}$.
>**Réponse**:
>On a que $(E)$ admet une infinité de solutions sur $\mathbb{R}^*$ mais une seule prolongeable par continuité, donc, $(E)$ n'admet que cette solution :
>$y = {F(x)\over x}$

## Partie II
On admet que $F$ admet une limite finie en $+\infty$. On cherche a determiner la valeur de cette limite.
Pour tout entier naturel $n$, on pose les suites $(I_n)$ et $(J_n)$ tel que :
$$
\begin{align}
I_n &= \int_0^{\pi\over2} {sin((2n+1)t) \over sin(t)}dt \\
J_n &= \int_0^{\pi\over2} {sin((2n+1)t) \over t}dt
\end{align}
$$
7. Montrer, par les [[Fonctions trigonométriques#Formule d'Euler|formules d'euler]] que pour tout $n \in \mathbb{N}^*$ et pour tout $t \in ]0, \pi[$,
$$
{sin((2n+1)t) \over sin(t)} = 1+2\sum_{k=1}^n cos(2kt)
$$
>**Réponses**:
>On rappel les formules d'Eulers :
>$sin(x) = (e^{ix} - e^{-ix}) / 2i$ et $cos(x) = (e^{ix} + e^{-ix}) / 2$
>On calcul a l'envers 

$$
\begin{align}
{sin([2n+1]t) \over sin(t)} 
&= { e^{[2n+1]ti} + e^{-[2n+1]ti} \over 2i} {2i \over e^{it} -e^{-it}} \\
&= { e^{[2n+1]ti} + e^{-[2n+1]ti}  \over e^{it} -e^{-it}} \\
&= 
\end{align}
$$

[^1]: Pour voir la méthode complète, voir [[Equations différentielles linéaires#Equation différentielle du premier ordre|Méthode]]. 