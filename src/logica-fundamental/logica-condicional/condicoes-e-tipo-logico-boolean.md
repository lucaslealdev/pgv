---
cover: >-
  https://images.unsplash.com/photo-1633613286848-e6f43bbafb8d?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwzfHxxdWVzdGlvbnxlbnwwfHx8fDE2ODkyMTA1NTB8MA&ixlib=rb-4.0.3&q=85
coverY: 57
---

# 🙆♀ Condições e tipo lógico (boolean)

{% hint style="success" %}
**Racional**: utilizando as condições é que você pode fazer com que o fluxo da estrutura condicional seja útil.
{% endhint %}

A condição é um conceito fundamental na estrutura condicional "if", pois determina o caminho que o código seguirá: o caminho do "if" ou o caminho do "else".

Para entender melhor, vamos conhecer um novo tipo de dado chamado boolean ou booleano. Esse tipo de dado possui apenas dois valores possíveis: verdadeiro ou falso. Ou seja, a condição pode ser "true" (verdadeira) ou "false" (falsa).

Para criar essas condições, utilizamos os operadores de comparação, como igual, maior que, menor que, entre outros. Esses operadores comparam valores e, como resultado, geram o valor booleano verdadeiro ou falso, indicando se a condição é atendida ou não.

Resumindo, o "if" é uma forma de fazer o código tomar decisões com base em condições que podem ser verdadeiras ou falsas, e essas condições são criadas usando operadores de comparação. Com essa compreensão, você estará preparado para usar a estrutura condicional "if" de forma eficiente em seus programas.

Abaixo a lista de operadores de comparação retirada da [documentação](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Expressions\_and\_Operators#operador\_comparacao) do JS.

<table data-full-width="true"><thead><tr><th width="274">Operador</th><th width="378.33333333333337">Descrição</th><th>Exemplos que retornam verdadeiro</th></tr></thead><tbody><tr><td>Igual (<code>==</code>)</td><td>Retorna verdadeiro caso os operandos sejam iguais.</td><td><code>3 == var1</code> <code>"3" == var1</code> <code>3 == '3'</code></td></tr><tr><td>Não igual (<code>!=</code>)</td><td>Retorna verdadeiro caso os operandos não sejam iguais.</td><td><code>var1 != 4</code> <code>var2 != "3"</code></td></tr><tr><td>Estritamente igual (<code>===</code>)</td><td>Retorna verdadeiro caso os operandos sejam iguais <strong>e do mesmo tipo</strong>. Veja também <a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Object/is"><code>Object.is</code></a> e <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness">igualdade em JS (en-US)</a>.</td><td><code>3 === var1</code></td></tr><tr><td>Estritamente não igual (<code>!==</code>)</td><td>Retorna verdadeiro caso os operandos não sejam iguais e/ou não sejam do mesmo tipo.</td><td><code>var1 !== "3"</code> <code>3 !== '3'</code></td></tr><tr><td>Maior que (<code>></code>)</td><td>Retorna verdadeiro caso o operando da esquerda seja maior que o da direita.</td><td><code>var2 > var1</code> <code>"12" > 2</code></td></tr><tr><td>Maior que ou igual (<code>>=</code>)</td><td>Retorna verdadeiro caso o operando da esquerda seja maior ou igual ao da direita.</td><td><code>var2 >= var1</code> <code>var1 >= 3</code></td></tr><tr><td>Menor que (<code>&#x3C;</code>)</td><td>Retorna verdadeiro caso o operando da esquerda seja menor que o da direita.</td><td><code>var1 &#x3C; var2</code> <code>"12" &#x3C; "2"</code></td></tr><tr><td>Menor que ou igual (<code>&#x3C;=</code>)</td><td>Retorna verdadeiro caso o operando da esquerda seja menor ou igual ao da direita.</td><td><code>var1 &#x3C;= var2</code> <code>var2 &#x3C;= 5</code></td></tr></tbody></table>

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
Aproveite para mudar o valor da constante <mark style="color:purple;">`numero`</mark> na linha 1, e ver a diferença na prática.
{% endhint %}

### Exemplo da função precoDaPipoca com a variação do tamanho:

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
