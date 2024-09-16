
> Ce chapitre nécessite de comprendre les notions de [[Valeur propre]], d'[[Espace vectoriel]] et de [[Polynomes]].
## Définition
Soit $f$ un endomorphisme de $E$, on dit qu'on **réduit** l'endomorphisme quand on trouve une base $B$ de $E$ tel que $Mat_B(f)$ soit diagonale. 

## Motivations
Les matrices diagonales sont plus faciles a manipuler. Ainsi, dans certain contextes comme les puissances de matrices ou les résolutions de systèmes [[Equations différentielles linéaires|différentiels]]. 

## Méthode
Dans toute la suite, on considère $f$ un endomorphisme de $E$, ainsi que $\chi_f$ le polynôme caractéristique. 
Soit $A$ la matrice associée a $f$ dans la base canonique. 
1. On calcul $\chi_f$. Si $\chi_f$ n'est pas scindé, **on arrête là**[^1], sinon, on note $\lambda_1, \lambda_2, ..., \lambda_n$ les [[Valeur propre|valeurs propres]] de $f$ et $m_{\lambda_1}, m_{\lambda_2}, ..., m_{\lambda_n}$ leurs multiplicités. 
2. Pour chaque espace propre $E_{\lambda_i}$ on calcul une base $\mathcal{B}_i$. Si, pour n'importe quel $i$, on a $dim(E_{\lambda_i}) < m_{\lambda_i}$, **on arrête là**.
3. On pose $\mathcal{B} = (\mathcal{B_1}, \mathcal{B_2}, ..., \mathcal{B_n})$. $\mathcal{B}$ est alors une base de $E$. Alors, on pose $\mathcal{C}$ la base canonique de $E$:
$$
D = P^{-1}AP\quad\text{avec}\quad P = P_{\mathcal{C}}^{\mathcal{B}}
$$
4. On trouve alors que $D$ est une matrice diagonale de la forme $D = Diag(\underbrace{\lambda_1,...,\lambda_1}_{m_{\lambda_1} \text{ fois} } , \underbrace{\lambda_2,...,\lambda_2}_{m_{\lambda_2} \text{ fois} },..., \underbrace{\lambda_n,...,\lambda_n}_{m_{\lambda_n} \text{ fois} })$. 

En des termes plus algorithmiques, on peu imaginer une fonction pour diagonaliser une matrice:
```python
def Diagonalisation(A):
	Xa = PolynomeCar(A) #Calcul le polynome caracteristique de A
	
	if not scinde(Xa): #si Xa n'est pas scindé, on stop
		print("A ne peut pas etre diagonalisée")
		return 
	
	#On obtien une liste des valeurs propres et de leurs multiplicités.
	vp, mul = ValeursPropres(Xa) 
	Bases = []
	diagonale = []
	for i in range(len(vp)):
		#EspacePropre retourne l'espace propre liée a une matrice et a 
		#une valeur propre.
		if dim(EspacePropre(A, vp[i])) < mul[i]):
			 print("A ne peut pas etre diagonaliser")
			 return
		else:
			Bases.append(EspacePropre(A, vp[i])).base)
			for j in range(mul[i]):
				diagonale.append(vp[i])
	
	D = Diag(diagonale)
	P = MatPassage(A, D)
	
	print("A a été diagonalisée")
	return (D,P)
```

----
[^1]: En effet, si le polynôme caractéristique n'est pas scindé sur $\mathbb{K}$, alors l'endomorphisme n'est pas diagonalisable. En voici la [[Preuve du CNS de diagonalisabilité|preuve]].