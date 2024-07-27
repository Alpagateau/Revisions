#mecanic
## Définition
Lorsque l'on étudie un système mécanique, il existes plusieurs façons de représenter la position d'un point dans l'espace. Dans tous les cas, un point est représenté par un tuplet ou un triplet (selon si on est en 2D ou 3D). Le **système de coordonnées** indique comment interpréter ces coordonnées. 

## Système cartésien
C'est le système le plus simple, le plus trivial. On écrit les coordonnées (x,y,z). 
![[cartesian_coordinates.png]]

## Système cylindrique
Si on étudie un mouvement de rotation autour d'un axe, il peut être utile de représenté un point a travers de coordonnées **cylindrique**, écrites ($r$, $\phi$, $z$)
![[cylindrical_coordinates.png|300]]
Avec $r$ étant le rayon du cylindre, $\phi$ étant l'angle entre le point et l'axe $e_x$, et $z$ la hauteur. A noter que $\rho$ est le vecteur unitaire a $\phi$ degrés de l'axe $e_x$. Ainsi :
$$
\rho = cos(\phi)e_x + sin(\phi)e_y
$$
Et de la on tiens : 
$$
P = r \rho + ze_z
$$
## Système sphérique
Si on étudie le mouvement d'une rotule ou de rotation autour d'une sphère, on peut utiliser des coordonnées sphériques, noté ($r, \theta, \phi$)
![[Pasted image 20240727184425.png|300]]
Avec $r$ le rayon de la sphère, $\phi$ l'axe "polaire" (par rapport a l'axe $e_x$), et $\theta$ la colatitude (par rapport a l'axe $e_z$)