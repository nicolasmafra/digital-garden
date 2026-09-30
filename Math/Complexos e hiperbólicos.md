## Unidades imaginárias
A unidade complexa se caracteriza por:

$i^2=-1$

Já a unidade hiperbólica, por:

$j^2 = 1, j \ne 1$

## Definição matricial
Como as unidades imaginárias não se misturam com as reais durante soma, elas agem como uma segunda dimensão. Assim, também conseguimos definir as unidades imaginárias atravéz de [[Matrizes]], o que é particularmente útil:

$$
1 \equiv I =
\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}
$$

$$
i \equiv J =
\begin{bmatrix}
0 & -1 \\
1 & 0
\end{bmatrix}
$$

$$
j \equiv K =
\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}
$$

Note que ambas são matrizes anti-diagonais. Isso garante que reais e imaginários atuem em dimensões diferentes.

E a partir dessas unidades, podemos criar os números complexos e hiperbólicos usando combinações lineares da matriz identidade e uma matriz de unidade imaginária:

$a +bi \equiv aI + bJ$
$a +bj \equiv aI + bK$

### Magnitude

Perceba que o determinante da matriz complexa é justamente o quadrado da magnitude do número complexo que ela representa.

### Conjugação
Perceba que a transposta da matriz complexa é justamente o conjugado do número complexo.