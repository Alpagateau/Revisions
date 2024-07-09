> Cette page est differente de la [[Logique]] et ne traite que des methodes de demonstrations

Les quatres grands types de raisonnements logiques pour montrer $P \Rightarrow Q$ sont:
- **Direct** : on suppose $P$ et on montre $Q$
- **Par contraposition** : on suppose $\overline{Q}$ et on montre $\overline{P}$
- **Disjonction de cas** : On suppose $P$ et on decompose chaque possibilités de $Q$
- **Par l'absurde** : On suppose $P$ et $\overline{Q}$ puis on cherche une contradiction
## Analyse synthèse
>**Analyse**
>On suppose $P$ et on deduit les propriété de la solutions
>**Synthèse**
>On verifie la possibilité de ces dites propriétés
>**Conclusion**
>On donne les solutions au probleme

## Principe de récurrence
### simple
>**Initialisation**
>On montre $P(n_0)$ pour $n_0 \in \mathbb{N}$
>**Hérédité**
>Soit $n$ tel que $P(n) = 1$, on montre $P(n+1)$
>**Conclusion**
>$\forall n > n_0, P(n) = 1$

### double
>**Initialisation**
>On montre $P(n_0)$ et $P(n_0 + 1)$ pour $n_0 \in \mathbb{N}$
>**Hérédité**
>Soit $n$ tel que $P(n) = 1$ et $P(n +1) = 1$, on montre $P(n+2)$
>**Conclusion**
>$\forall n > n_0, P(n) = 1$

### forte
>**Initialisation**
>On montre $P(n_0)$ pour $n_0 \in \mathbb{N}$
>**Hérédité**
>Soit $n$ tel que $\forall k \in [n_0, n], P(k) = 1$, on montre $P(n+1)$
>**Conclusion**
>$\forall n > n_0, P(n) = 1$

