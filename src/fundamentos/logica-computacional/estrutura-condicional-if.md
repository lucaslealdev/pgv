---
cover: >-
  https://images.unsplash.com/photo-1548147963-30ac0d3d7723?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxwYXRoc3xlbnwwfHx8fDE2ODkwMDI3ODJ8MA&ixlib=rb-4.0.3&q=85
coverY: 198
---

# 🤔 Estrutura condicional if

{% hint style="success" %}
**Vantagem:** as estruturas condicionais como um todo permitem que o seu código tome decisões automaticamente, variando as linhas que serão ou não serão executadas.
{% endhint %}

Você viu como criar funções, e isso já permite reutilizar muito o código. Mas isso ainda não te dá poder de **variar** o que acontece no seu código.

Por exemplo, é comum o preço de um alimento variar conforme o tamanho da porção. Se você criar uma função que retorna o preço de um pedido em um carrinho de pipoca, sem estruturas condicionais você só poderá variar o preço conforme a quantidade, mas não conforme o tamanho.

### Exemplo sem a variação do tamanho:

{% code lineNumbers="true" %}
```javascript
const precoDaPipoca = (quantidade) => {
  return (quantidade * 3.50).toFixed(2);
};
console.log(`Três saquinhos de pipoca custam R$${precoDaPipoca(3)}`);
console.log(`Quatro saquinhos de pipoca custam R$${precoDaPipoca(4)}`);
console.log(`Um saquinho de pipoca custa R$${precoDaPipoca(1)}`);
```
{% endcode %}

{% hint style="info" %}
Siga [este link](https://coolfee.github.io/#\{%22code%22:%22const%20precoDaPipoca%20=%20\(quantidade\)%20=%3E%20{\n%20%20return%20\(quantidade%20\*%203.50\).toFixed\(2\);\n};\nconsole.log\(%60Tr%C3%AAs%20saquinhos%20de%20pipoca%20custam%20R\$${precoDaPipoca\(3\)}%60\);\nconsole.log\(%60Quatro%20saquinhos%20de%20pipoca%20custam%20R\$${precoDaPipoca\(4\)}%60\);\nconsole.log\(%60Um%20saquinho%20de%20pipoca%20custa%20R\$${precoDaPipoca\(1\)}%60\);%22,%22tests%22:%22;%22}) para visualizar o código acima.
{% endhint %}

### Sintaxe do if

A sintaxe do if, ou seja a forma como você deve digitar o comando, é essa:

```javascript
if (<condição>) {
  //código que executa quando a condição é verdadeira
} else {
  //código que executa quando a condição é falsa
}
```

{% hint style="info" %}
<mark style="color:green;">`If`</mark> vem do inglês e significa <mark style="color:green;">`se`</mark>, e <mark style="color:green;">`else`</mark> significa <mark style="color:green;">`senão`</mark>. Ou seja, esse código pode ser lido como <mark style="color:green;">`se talcoisa, então faça esse algo; senão faça esse outro algo`</mark>.
{% endhint %}

É importante notar que:

1. **Não é obrigatório** o uso da cláusula `else`, a estrutura pode acabar no primeiro fechamento de chaves (`}`).
2. Como o `else` significa `senão`, o código dentro do `else` não executa caso entre na condição do `if`. Ou seja eles são excludentes, **ou é um ou é o outro**. Caso você queira que algo aconteça independentemente da condição, basta **não** colocar o código dentro da estrutura do `if` ou do `else`.
3. A condição precisa seguir a sintaxe correta do JavaScript.

### A condição

A condição é um elemento importantíssimo da estrutura condicional _if_, pois é o que determina qual caminho o código vai seguir (o caminho do _if_ ou o caminho do _else_).

<div data-full-width="false">

<figure><img src="../../.gitbook/assets/.png" alt=""><figcaption></figcaption></figure>

</div>

Para criar condições você usa os operadores de comparação, que são **igual**, **maior que**, **menor que**, dentre outros, e todos no fim geram um valor verdadeiro ou falso. Para a computação, não existe _parecido**,**_ apenas igual ou diferente (com uma exceção)_**.**_ Leia [esse artigo](https://web.archive.org/web/https://www.alura.com.br/artigos/operadores-matematicos-em-javascript) do site Alura para obter uma explicação rápida sobre os operadores.

Abaixo a lista de operadores de comparação retirada da [documentação](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Expressions\_and\_Operators#operador\_comparacao) do JS.

<table data-full-width="true"><thead><tr><th width="274">Operador</th><th width="378.33333333333337">Descrição</th><th>Exemplos que retornam verdadeiro</th></tr></thead><tbody><tr><td>Igual (<code>==</code>)</td><td>Retorna verdadeiro caso os operandos sejam iguais.</td><td><code>3 == var1</code> <code>"3" == var1</code> <code>3 == '3'</code></td></tr><tr><td>Não igual (<code>!=</code>)</td><td>Retorna verdadeiro caso os operandos não sejam iguais.</td><td><code>var1 != 4</code> <code>var2 != "3"</code></td></tr><tr><td>Estritamente igual (<code>===</code>)</td><td>Retorna verdadeiro caso os operandos sejam iguais e do mesmo tipo. Veja também <a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Object/is"><code>Object.is</code></a> e <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness">igualdade em JS (en-US)</a>.</td><td><code>3 === var1</code></td></tr><tr><td>Estritamente não igual (<code>!==</code>)</td><td>Retorna verdadeiro caso os operandos não sejam iguais e/ou não sejam do mesmo tipo.</td><td><code>var1 !== "3"</code> <code>3 !== '3'</code></td></tr><tr><td>Maior que (<code>></code>)</td><td>Retorna verdadeiro caso o operando da esquerda seja maior que o da direita.</td><td><code>var2 > var1</code> <code>"12" > 2</code></td></tr><tr><td>Maior que ou igual (<code>>=</code>)</td><td>Retorna verdadeiro caso o operando da esquerda seja maior ou igual ao da direita.</td><td><code>var2 >= var1</code> <code>var1 >= 3</code></td></tr><tr><td>Menor que (<code>&#x3C;</code>)</td><td>Retorna verdadeiro caso o operando da esquerda seja menor que o da direita.</td><td><code>var1 &#x3C; var2</code> <code>"12" &#x3C; "2"</code></td></tr><tr><td>Menor que ou igual (<code>&#x3C;=</code>)</td><td>Retorna verdadeiro caso o operando da esquerda seja menor ou igual ao da direita.</td><td><code>var1 &#x3C;= var2</code> <code>var2 &#x3C;= 5</code></td></tr></tbody></table>

Para utilizar esses operadores você os insere dentro dos parênteses do `if` e pode colocar variáveis e/ou valores fixos na comparação. Quando a comparação dá verdadeira, o código executa o bloco do `if`, caso dê falsa o código executa o bloco do `else`.

Eis um exemplo para fins didáticos:

{% code lineNumbers="true" %}
```javascript
const numero = 3;

if (numero === 3) { //isso dá verdadeiro
  console.log('O número é 3.'); //essa linha executa
} else {
  console.log('O número não é 3.'); //essa linha NÃO executa
}
```
{% endcode %}

{% hint style="info" %}
Siga [este link](https://coolfee.github.io/#\{%22code%22:%22const%20numero%20=%203;\n\nif%20\(numero%20===%203\)%20{\n%20%20console.log\('O%20n%C3%BAmero%20%C3%A9%203.'\);\n}%20else%20{\n%20%20console.log\('O%20n%C3%BAmero%20n%C3%A3o%20%C3%A9%203.'\);\n}%22,%22tests%22:%22;%22}) para ver o código executando.\
Aproveite para mudar o valor da constante `numero` na linha 1, e ver a diferença na prática.
{% endhint %}

### Exemplo com a variação do tamanho:

{% code lineNumbers="true" %}
```javascript
const precoDaPipoca = (quantidade, tamanho) => {
  if (tamanho === 'P') {
    return (quantidade * 3.50).toFixed(2);
  }
  if (tamanho === 'M') {
    return (quantidade * 4).toFixed(2);
  }
  if (tamanho === 'G') {
    return (quantidade * 5).toFixed(2);
  }
};
console.log(`Três saquinhos de pipoca custam R$${precoDaPipoca(3, 'G')}`);
console.log(`Quatro saquinhos de pipoca custam R$${precoDaPipoca(4, 'P')}`);
console.log(`Um saquinho de pipoca custa R$${precoDaPipoca(1, 'M')}`);
```
{% endcode %}
