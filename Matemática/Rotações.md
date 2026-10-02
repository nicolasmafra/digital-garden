---
dg-publish: true
---
## Introdução
As rotações, tanto as circulares como as hiperbólicas, aparecem relacionadas a exponenciais com números complexos por que será?

Ao final, é interessante notar que as funções trigonométricas e hiperbólicas são apenas os pedaços par e ímpar da rotação.

## Origem da rotação
Uma rotação consiste em mover suavemente um ponto que está em uma dimensão em direção a outra dimensão perpendicular. Portanto, seu domínio é um plano, 2 dimensões.

A rotação mais simples por ser pensada como um ciclo de direções dessas dimensões:

+x, +y, -x, -y

Isso lembra algo? Veja:

+1, +i, -1, -i

É exatamente a potenciação da unidade imaginária. Portanto, a rotação pode ser vista como uma interpolação dessa potenciação de imaginários.
## Relacionamento
Em resumo, uma rotação é o resultado de juntar a [[Exponencial]] com [[Números imaginários]]. Ao usar formato de matriz, fica mais nítido que a decomposição de cada dimensão coincide com a decomposição em partes par e ímpar.

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

## G=1

$$\frac{e^{x}+e^{-x}}{2}=\cosh(x)$$

$$\frac{e^{x}-e^{-x}}{2}=\sinh(x)$$

$$e^x=\cosh(x)+\sinh(x)$$

## G=j

$$\frac{e^{xj}+e^{-xj}}{2}=\cosh(x)$$

$$\frac{e^{xj}-e^{-xj}}{2}=j\sinh(x)$$

$$e^{xj}=\cosh(x)+j\sinh(x)$$

## G=i

$$\frac{e^{xi}+e^{-xi}}{2}=\cos(x)$$

$$\frac{e^{xi}-e^{-xi}}{2}=i\sin(x)$$

$$e^{xi}=\cos(x)+i\sin(x)$$

## Próximos passos
Por que a rotação preserva a magnitude dos números complexos? Por que ela é linear? Por que a inversão do ângulo a transforma em sua inversa e por que também é sua transposta?

Tem propriedades demais para ser considerado mera coincidência. Qual a evolução de complexidade que decorre nessas propriedades?

E quando tem mais de 2 dimensões, por que a matriz geradora deixa de ser uma unidade imaginária? Na verdade era para ser a direção da variação e não a unidade? Nesse caso foi mera coincidência?
