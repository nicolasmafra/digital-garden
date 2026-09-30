---
publish: true
created: 2026-06-06T09:28:06.582-03:00
modified: 2026-09-30T01:37:51.761-03:00
---

Em resumo, é o resultado de juntar a [[Exponencial]] com números [[Complexos e hiperbólicos]] e decompor em partes par e ímpar.

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

Podemos também obter essas funções através da decomposição da exponencial em par e ímpar:

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

$\frac{e^{x}+e^{-x}}{2}=\cosh(x)$

$\frac{e^{x}-e^{-x}}{2}=\sinh(x)$

$e^x=\cosh(x)+\sinh(x)$

## G=j

$\frac{e^{xj}+e^{-xj}}{2}=\cosh(x)$

$\frac{e^{xj}-e^{-xj}}{2}=j\sinh(x)$

$e^{xj}=\cosh(x)+j\sinh(x)$

## G=i

$\frac{e^{xi}+e^{-xi}}{2}=\cos(x)$

$\frac{e^{xi}-e^{-xi}}{2}=i\sin(x)$

$e^{xi}=\cos(x)+i\sin(x)$
