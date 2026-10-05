---
dg-publish: true
---
## Introdução
As rotações, tanto as circulares como as hiperbólicas, aparecem relacionadas a exponenciais com números complexos
 Por que será?

Ao final, é interessante notar que as funções trigonométricas ou hiperbólicas são apenas os pedaços par e ímpar da rotação em um plano.

## Generalização de algo mais básico
A rotação mais simples consiste em, dado um par de dimensões, permutar as unidades dessas dimensões de alguma forma que as duas dimensões interajam. A rotação circular (elíptica), por exemplo:

+x, +y, -x, -y

Isso lembra algo? Veja:

+1, +i, -1, -i

É exatamente a potenciação da unidade imaginária. Portanto, a rotação pode ser vista como uma generalização contínua dessa potenciação de [[Números imaginários]].

## Características essenciais
A rotação é uma transformação suave de um vetor, portanto podemos enxergar a variação (derivada) em cada ponto.

Essa variação tem duas propriedades importantes: preserva a magnitude do vetor e o deslocamento em cada ponto é proporcional à magnitude.

Por ser proporcional, é linear e a solução será uma [[Exponencial]], onde o expoente é o fator, que dita a direção e a velocidade. Por ser linear, podemos tratar o fator como uma [[Matrizes|matriz]]. Podemos tratar a velocidade como um fator real multiplicando uma matriz fixa. Como falta a direção, a matriz basicamente só diz a direção e o tipo da variação. Essa matriz é chamada de **geradora** da transformação.

Para manter a magnitude constante, o movimento precisa ser perpendicular à direção que aumenta a magnitude. Como é uma generalização da potenciação da unidade imaginária, essa matriz se comporta de maneira similar à unidade imaginária. Na verdade, quando todas as dimensões estão sendo usadas na rotação (dimensão par e toda direção é alterada), a matriz geradora coincide justamente com uma unidade imaginária.
## Transformação finita
Sabendo que a rotação é a [[Exponencial]] de [[Números imaginários]], ao usar formato de [[Matrizes]], fica mais nítido que a decomposição de cada dimensão coincide com a decomposição em partes par e ímpar.

Como dica, pense na parte real como a dimensão em que a transformação inicia e a imaginária como a segunda.

Relembrando a decomposição em série da exponencial:

$$
e^{xG}=
\sum_{n=0}^{\infty}\frac{(xG)^n}{n!}
$$
Ao aplicar uma unidade imaginária como geradora, os termos pares serão reais e os ímpares serão imaginários:

$$
\operatorname{Re}(e^{xG}) =
\sum_{n=0}^{\infty}\frac{(xG)^{2n}}{2n!}
$$

$$
G\operatorname{Im}(e^{xG}) =
\sum_{n=0}^{\infty}\frac{(xG)^{2n+1}}{(2n+1)!}
$$

Podemos também obter essas funções através da decomposição da exponencial em par e ímpar diretamente, sem necessitar da série:

$$
\operatorname{Re}(e^{xG}) =
\frac{e^{xG} + e^{-xG}}{2}
$$

$$
G \operatorname{Im}(e^{xG}) =
\frac{e^{xG} - e^{-xG}}{2}
$$
$$
e^{xG} =
\operatorname{Re}(e^{xG}) +
G \operatorname{Im}(e^{xG})
$$

Ao substituir G, temos:

### G=1, somente para ilustrar

$$\frac{e^{x}+e^{-x}}{2}=\cosh(x)$$

$$\frac{e^{x}-e^{-x}}{2}=\sinh(x)$$

$$e^x=\cosh(x)+\sinh(x)$$

### G=j, agora com duas dimensões

$$\frac{e^{xj}+e^{-xj}}{2}=\cosh(x)$$

$$\frac{e^{xj}-e^{-xj}}{2}=j\sinh(x)$$

$$e^{xj}=\cosh(x)+j\sinh(x)$$

### G=i, alternância extra

$$\frac{e^{xi}+e^{-xi}}{2}=\cos(x)$$

$$\frac{e^{xi}-e^{-xi}}{2}=i\sin(x)$$

$$e^{xi}=\cos(x)+i\sin(x)$$

## Próximos passos
Por que a inversão do ângulo a transforma em sua inversa e por que também é sua transposta? Qual a relação com a métrica do espaço?
