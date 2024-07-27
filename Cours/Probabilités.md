#probability
## Définition
On appel **probabilité** d'un évènement un réel compris entre 0 et 1. Plus ce nombre tends vers 1, plus la `chance` que cet événement se produise est grande.
Les probabilités ont un fort lien avec l'étude des [[Ensembles|ensembles]] mais n'utilisent pas le même vocabulaire. 
Cette proximité avec les ensembles amène au fait que les [[Ensembles#Opérations entre ensembles|operations]] entre ensembles et entre évènements sont les mêmes. 

## Vocabulaire

| Terme probabilistique | Terme ensembliste        |        Notation mathématique        |
| --------------------- | ------------------------ | :---------------------------------: |
| Univers               | Ensemble entier          |              $\Omega$               |
| Évènement impossible  | Ensemble vide            |             $\emptyset$             |
| Résultat d'expérience | Élément de $\Omega$      |         $\omega \in \Omega$         |
| Évènement élémentaire | Singleton                |            $\{\omega\}$             |
| Tribu                 | Ensemble de sous parties |   $\mathcal{T} \subset P(\Omega)$   |
| Évènement             | Sous-ensemble ou partie  |         $A \in \mathcal{T}$         |
| Evenement contraire   | Complémentaire           |       $A^c, A\in \mathcal{T}$       |
| A ou B                | Union de A et B          | $A \cup B, (A,B) \in \mathcal{T}^2$ |
| A et B                | Intersection A et B      | $A \cap B, (A,B)\in \mathcal{T}^2$  |
| A implique B          | A inclus dans B          |            $A \subset B$            |
| A et B incompatibles  | A et B disjoints         |       $A \cap B = \emptyset$        |
| $\omega$ réalise A    | $\omega$ inclus dans A   |           $\omega \in A$            |
On appel **expérience aléatoire** une expérience pouvant être répété dans les mêmes conditions plusieurs fois et dont l'issue dépend du hasard. 
On appel **univers** l'ensemble des issues possibles d'une telle expérience. 

## Fonction probabilité
On appel **probabilité** toute fonction de $\mathcal{T}$ dans $[0,1]$ qui vérifie :
- $\forall A \in \mathcal{T}, \quad \mathbb{P}(A) \ge 0$
- $\mathbb{P}(\Omega) = 1$
- $\forall (A, B) \in \mathcal{T}^2, A \cap B = \emptyset, \quad \mathbb{P}(A \cup B) = \mathbb{P}(A) + \mathbb{P}(B)$
On appel alors un triplet ($\Omega$, $\mathcal{T}$, $\mathbb{P}$) un **espace probabilisé**.
> $\mathbb{P}(A) = 0 \not \Rightarrow A = \emptyset \quad \quad \mathbb{P}(A) = 1 \not \Rightarrow A = \Omega$

## Propriétés élémentaires des proba
1. $\mathbb{P}(\emptyset) = 0$
2. $\mathbb{P}(A^c) = 1-\mathbb{P}(A)$
3. $A \subset B \Rightarrow \mathbb{P}(A) \le  \mathbb{P}(B)$
4. $\mathbb{P}(A \cup B) = \mathbb{P}(A) + \mathbb{P}(B) - \mathbb{P}(A \cap B)$

## Probabilité conditionnelles 
On appel la probabilité de A **sachant** B la probabilité de A relativement a B. On la note ainsi :
$$
\mathbb{P}(A|B) = {\mathbb{P}(A \cup B) \over \mathbb{P}(B)}
$$
## Théorèmes fondamentaux
1. Probabilités composés
$$
\begin{align}
\text{Soient }& A_0, A_1, A_2...A_n \\
\text{tels que } &\mathbb{P}(A_0 \cap A_1 \cap A_2 ... \cap A_n) \ne 0 \\
\mathbb{P}(A_0 \cap A_1 \cap A_2 ... \cap A_n) &= \mathbb{P}(A_0)\mathbb{P}(A_1|A_0)\mathbb{P}(A_2|A_1\cap A_0)...\mathbb{P}(A_n|A_{n-1}...\cap A_2 \cap A_1 \cap A_0)
\end{align}
$$

2. Probabilités complètes
$$
\displaystyle
\begin{align}
\forall(A_i)_{i \in \mathbb{N}} & \text{ tel que } \forall (i, j) \in \mathbb{N}, A_i \cap A_j =  \emptyset \\
\bigcup_{k=0}^n  A_k = \Omega
\end{align}
$$
On appel un tel $(A_i)$ système compet déventements.

