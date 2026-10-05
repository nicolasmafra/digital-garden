---
dg-publish: true
---
## Introdução

É interessante como exponencial de números imaginários produzem rotações. Também é curioso como matrizes expressam incrivelmente bem algumas de suas necessidades.

É possível também juntar 3 unidades e produzir os quaternions, que possuem propriedades similares a rotações 3D e se assemelham às dimensões do plano espaço-tempo.

Além disso, o Lorentz Boost da relatividade é considerado uma rotação hiperbólica, que usa números hiperbólicos, uma variação dos complexos.

E também existem os duais, que se assemelham a unidades diferenciais, embora seja bem diferente das demais.

Por que será que se relacionam assim?

## Unidades imaginárias
A unidade complexa se caracteriza por:

$i^2=-1$

Já a unidade hiperbólica, por:

$j^2 = 1, j \notin \mathbb{R}$

E a unidade dual:

$\epsilon^2 = 0, \epsilon \notin \mathbb{R}$

Em todos os casos, a unidade imaginária não faz parte dos números reais, atuando de forma isolada na adição como se fosse uma nova dimensão. Seu quadrado, no entanto, produz um número real, sendo essa a única diferença entre elas.

Os complexos nada mais são que a soma de ambas as dimensões. Perceba também que várias propriedades dos reais são preservadas, como associatividade e linearidade.
## Produto discreto
Podemos dar um passo para trás e analisar apenas o que acontece com o produto entre as unidades reais e imaginárias, em vez de todos os número complexos, já que são apenas as combinações lineares das unidades.

Multiplicar por 1 não altera nada. Multiplicar por -1 inverte e, se aplicado novamente, volta. Já ao multiplicar por uma unidade imaginária tem comportamento específico (iniciando em +1):

Os complexos fazem um ciclo de tamanho 4, que é +1, +i, -1, -i, ...

No caso dos hiperbólicos, fazem um ciclo de tamanho 2, que é +1, +j, ...

Já os duais, degeneram em zero após o segundo termo: +1, +e, 0, ...

## Definição matricial
Por falar em múltiplas dimensões e linearidade, as [[Matrizes]] são justamente isso. Portanto, é particularmente útil representar cada unidade real e imaginária como uma matriz, que preserva o comportamento do quadrado:

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

$$
\epsilon \equiv E =
\begin{bmatrix}
0 & 1 \\
0 & 0
\end{bmatrix}
$$

Note que as imaginárias são matrizes anti-diagonais. Isso garante que reais e imaginários atuem em dimensões diferentes na adição.

E a partir dessas unidades, podemos criar os números complexos, hiperbólicos e duais usando combinações lineares da matriz identidade e uma matriz de unidade imaginária:

$a +bi \equiv aI + bJ$
$a +bj \equiv aI + bK$
$a +b\epsilon \equiv aI + bE$

Para unificar complexo e hiperbólico, podemos criar um parâmetro s pode ser +1 ou -1:

$$
M = \begin{bmatrix}
0 & s \\
1 & 0
\end{bmatrix}
$$
### Determinante

Perceba que o determinante da matriz complexa ou hiperbólicas é justamente o quadrado da magnitude do número complexo que ela representa.

$$ det(aI + bM)=a^2 - sb^2 $$
$$ det(aI+bJ)=a^2 + b^2 $$
$$ det(aI+bK)=a^2 - b^2 $$

### Transposta
Perceba que a transposta da matriz complexa é justamente o conjugado do número complexo.

$$ (aI+bM)^t=aI+bM^t=aI+sbM $$

$$ (aI+bJ)^t=aI-bJ $$
## Potenciação
Como o quadrado de um número imaginário é um número real, ao elevar a unidade imaginária a um expoente par sempre será um número real, enquanto expoente ímpar dá número imaginário.

Além disso, as unidades imaginárias (com exceção da dual) voltam a si mesmas após 2 ou 4 potenciações, gerando ciclos.

Isso cria uma paridade cíclica interessante que pode ser observada na série de Taylor da [[Exponencial]], ao fornecer um número imaginário como parâmetro.

## Conjugação
Sabendo da paridade entre real e imaginário, podemos decompor um número em parte par e ímpar, sendo necessário apenas uma operação que inverta a parte ímpar (imaginária), chamada conjugação:

$Re(z)+i.Im(z) = z$
$Re(z)-i.Im(z)=z^*$

$$
Re(z) = \frac{z+z^*}{2}
$$
$$
i.Im(z) = \frac{z-z^*}{2}
$$
