#algebra 
Le pivot de Gauss est une méthode qui permet de résoudre des [[Systèmes linéaires]] et d'inverser des [[Matrices]].

## Méthode
>On commence a la premiere colonne, premiere ligne. En utilisant les operations élémentaires, on échelonne le système. 
>Dans le cas d'une inversion de matrice, on effectue l'échelonnage en remonté aussi.

```python
S = #un tableau avec les coefficients de 
    #la matrice ou du systeme a inverser
    #de taille (n,p)

for i in range(n):
	S[i] = S[i] / S[i][i]
	for j in range(i, n):
		S[j] -= S[j][i] * S[i]  
```

