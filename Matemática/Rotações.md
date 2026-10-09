---
dg-publish: true
---
## Introdução
As rotações, tanto as circulares como as hiperbólicas, aparecem relacionadas a exponenciais com números complexos
 Por que será?

Ao final, é interessante notar que as funções trigonométricas ou hiperbólicas são apenas os pedaços par e ímpar da rotação em um plano.

## Origem física
Uma transformação rígida é uma isotopia suave e isométrica durante toda a transformação. Essa transformação é afim, significando que pode ser decomposta em translação e uma outra que é linear. Essa outra é justamente a rotação.

Isso é o que se espera fisicamente, mas até a estrutura física emerge de estruturas mais simples que possuem as mesmas propriedades essenciais.

## Estrutura mais básica
A rotação mais básica consiste em, dado um par de dimensões perpendiculares por definição, permutar linearmente as unidades dessas dimensões. A rotação circular (elíptica), por exemplo:

+x, +y, -x, -y

Isso lembra algo? Veja:

+1, +i, -1, -i

É equivalente à potenciação da unidade [[Números imaginários|imaginária]]. Generalizando para incluir a hiperbólica, um eixo vai para outro diferente e volta, podendo ou não voltar com sinal invertido (na hiperbólica o sinal se mantém, resultando em 2 swaps).

Portanto, a rotação pode ser vista como uma generalização dessa estrutura, acrescentando continuidade e preservação de distância.
## Características essenciais
A rotação é uma transformação contínua de um vetor, que é um ponto em relação a uma origem. Então em cada ponto há uma variação (derivada direcional). Essa variação tem duas propriedades importantes: preserva a magnitude e varia proporcionalmente a ela.

Como a variação do vetor é proporcional a si mesmo, a solução é uma [[Exponencial]], onde o expoente é o fator que dita a variação. Além disso é linear e podemos tratar o fator como uma [[Matrizes|matriz]], decompondo um fator real (ângulo) multiplicando uma matriz fixa. Essa matriz basicamente diz qual a direção da variação em relação à direção do vetor. Essa matriz é chamada de **geradora** da transformação.

Para manter a magnitude constante, o movimento precisa ser perpendicular à direção do próprio vetor. Note que exponenciar com essa matriz generaliza a ação de multiplicar por uma unidade imaginária. Na verdade, quando todas as dimensões estão sendo usadas na rotação (dimensão par e toda direção é alterada), a matriz geradora coincide justamente com uma unidade imaginária do espaço.
## Transformação finita
Sabendo que a rotação é a [[Exponencial]] de [[Números imaginários]], ao usar formato de [[Matrizes]], fica mais nítido que a decomposição de cada dimensão coincide com a decomposição em partes par e ímpar.

Como dica, pense na parte real como a dimensão em que a transformação inicia (ângulo zero) e a imaginária como a direção da variação naquele ponto inicial.

Relembrando a decomposição em série da exponencial:

$$
e^{xG}=
\sum_{n=0}^{\infty}\frac{(xG)^n}{n!}
$$
Ao aplicar uma unidade imaginária como geradora, os termos pares serão reais e os ímpares serão imaginários:

$$
\sum_{n=0}^{\infty}\frac{(xG)^{2n}}{2n!}
= \operatorname{Re}(e^{xG})
$$

$$
\sum_{n=0}^{\infty}\frac{(xG)^{2n+1}}{(2n+1)!}
= G\operatorname{Im}(e^{xG})
$$

Podemos também decompor a exponencial em par e ímpar diretamente, usando só a exponencial inversa, sem necessitar da série:

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
