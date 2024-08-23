## Définition
Les **règles de Slater** sont un ensemble de règles empiriques qui permettent d’évaluer la **charge nucléaire effective** d'un atome. 

## Fonction écran
L'[[Energie d'ionisation]] dépend non seulement de la charge réelle[^1], mais aussi d'une **fonction écran** qui atténue la charge réelle. Celle ci provient des electrons se repoussant les uns les autres.  On établie alors cette fonction grace a la [[Configuration Atomique|configuration atomique]]. 
On écrit alors, que la charge effective $\mathbb{Z}^*$ tel que :
$$
\mathbb{Z}^* = \mathbb{Z} - \sigma
$$
avec $\mathbb{Z}$ la charge réelle et $\sigma$ la fonction écran. 
## Méthode de calcul
Les électrons sont placés un a un dans l'ordre d'abord du [[Nombres quantiques|nombre quantique]] $n$ puis $l$. A l’exception des couches s et p ($l$ = 0 et $l$ = 1) sont conservés ensembles. 
>On obtiens alors **1s; 2s2p; 3s3p; 3d; 4s4p; 4d; 4f**...

La fonction écran $\sigma_j$ de l'électron $j$ est la somme des fonctions écran $\sigma_{i \to j}$ exercé sur $j$ par tout autre électron $i$. 
Voici l'algorithme :
```python
class electron:
	int n;
	int l;
	int mL;
	int mS; // 1 ou -1

def sigma(elecList,elecEtudier)
{
	
}

```