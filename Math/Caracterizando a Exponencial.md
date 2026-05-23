## Definição aritmética
Assim como a multiplicação é uma repetição da adição, a potenciação é repetição da multiplicação.
Por esse motivo, ela possui propriedades distributivas que a caracterizam:

$$
a^{b+c} = a^b a^c
$$

No entanto, a potenciação é uma operação binária. Para se tornar exponencial, é necessário um currying: primeiro é fixado um valor para a base da potência, em seguida se parametriza o expoente e a trata como função de um único parâmetro:

$$
f(x) = a^x
$$

## Característica funcional
A exponencial é a única função com as seguintes propriedades, já observadas na definição aritmética:
- $f(x+y) = f(x)f(y)$
- $f(0) = 1$

Onde a segunda propriedade só é necessária para evitar a solução trivial $f(x) = 0$

## Característica diferencial
A partir da característica funcional, é fácil usar a definição de derivada para provar que a derivada de uma exponencial é proporcional à própria derivada:

$$
f'(x) = c f(x)
$$

## Base natural
Existe uma base específica que torna a constante de proporcionalidade igual a 1. Essa base é chamada de base natural, ou número de Euler. Inclusive, muitas vezes o termo "exponencial" é usado especificamente para a exponencial de base natural:

$$
f(x) = \exp(x) = e^x \iff f'(x) = f(x)
$$

## Definição por série
Sabendo que qualquer derivada enésima da exponencial continua sendo ela mesma, podemos calcular a exponencial usando a série de Taylor:

$$
\exp(x)=\sum_{n=0}^{\infty}\frac{x^n}{n!}
$$
E podemos usá-la para calcular a base natural:

$$
e=\exp(1)=\sum_{n=0}^{\infty}\frac{1}{n!}
$$
