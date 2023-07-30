---
cover: >-
  https://images.unsplash.com/photo-1548147963-30ac0d3d7723?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxwYXRoc3xlbnwwfHx8fDE2ODkwMDI3ODJ8MA&ixlib=rb-4.0.3&q=85
coverY: 198
---

# 🤔 Estrutura condicional if

{% hint style="success" %}
**Vantagem:** as estruturas condicionais como um todo permitem que o seu código tome decisões automaticamente, variando as linhas que serão ou não serão executadas.
{% endhint %}

No módulo anterior, você aprendeu como criar funções, o que já é ótimo para reutilizar o código. No entanto, essa abordagem ainda não lhe proporciona flexibilidade para lidar com variações no comportamento do código.

Vamos tomar como exemplo o preço de um alimento que pode variar de acordo com o tamanho da porção. Suponha que você tenha criado uma função para calcular o preço de um pedido em um carrinho de pipoca. Sem o uso de estruturas condicionais, você pode variar o preço conforme a quantidade (ao multiplicar), mas não seria possível ajustar o preço de acordo com o tamanho da porção.

Em outras palavras, as estruturas condicionais são fundamentais para permitir que seu código tome decisões e se adapte a diferentes situações. Elas possibilitam criar lógicas que levam em consideração condições específicas, como o tamanho da porção no exemplo mencionado. Dessa forma, você ganha o poder de tornar seu código mais inteligente e capaz de lidar com uma ampla gama de cenários, tornando-o mais versátil e útil em diversas situações. Com o conhecimento das estruturas condicionais, você estará preparado para criar soluções mais sofisticadas e adequadas às necessidades do seu programa.

### Exemplo limitado sem o uso de IF:

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

Agora você vai estudar o `if` e na próxima lição verá uma exemplo da função `precoDaPipoca` com o uso dessa estrutura condicional muito importante.

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
2. Como o `else` significa `senão`, o código dentro do `else` **não executa** caso entre na condição do `if`. Ou seja eles são excludentes, **ou é um ou é o outro**. Caso você queira que algo aconteça independentemente da condição, basta **não** colocar o código dentro da estrutura do `if` ou do `else`.
3. A condição precisa seguir a sintaxe correta do JavaScript.

E quais condições podemos utilizar? Isso veremos na nossa próxima lição.
