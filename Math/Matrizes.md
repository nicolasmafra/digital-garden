Matriz parece ser toda uma estrutura complicada e arbitrária, mas pode ser naturalmente entendida se tratada como função lambda.

Os dados internos da matriz podem ser pensados como uma função que recebe 2 índices e retorna um número:

$$
M \equiv (a,b) \mapsto M_{a,b}
$$

A soma de duas matrizes pode ser pensada como a soma simples, associando os índices como se fossem os mesmos para ambas as matrizes:

$$
M+N \equiv
(a,b) \mapsto M_{a,b}+N_{a,b}
$$

A multiplicação de matriz por número pode ser pensada trivialmente como apenas internalizando o número:

 $$
kM \equiv
(a,b) \mapsto kM_{a,b}
$$

A multiplicação de duas matrizes pode ser pensada como duas etapas: multiplicação simples e somatória iterando os valores do índice contraído:

$$
MN \equiv (a,c) \mapsto
\sum_{b} M_{a,b}N_{b,c}
$$

Até o momento, a única parte complicada é justamente essa contração com somatória.
## Vetor
Vetores podem ser pensados como matriz coluna, que é onde um dos índices tem apenas um valor possível e por isso não precisa ser parâmetro:

$$
v \equiv (a) \mapsto v_{a,1}
$$
O mesmo se aplica para covetor (matriz linha), bastando fixar o primeiro índice em vez do segundo.

Com essa definição, tratando vetores como matrizes, já sabemos multiplicar matrizes com vetores.

## Linearidade
Linearidade é a propriedade mais importante de uma matriz. Relembrando as condições:

$f(x+y) = f(x) + f(y)$

$f(kx) = kf(x)$

No caso de matriz, ela é linear quando aplicada a um vetor:

$$
f(v) = Mv \equiv
(a) \mapsto \sum_b M_{a,b}v_b
$$
Como internamente estamos usando uma multiplicação simples, que distribui sobre a adição e é associativa, a função em si também é linear, portanto a matriz é linear.