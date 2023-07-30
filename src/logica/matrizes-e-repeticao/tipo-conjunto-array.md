---
cover: >-
  https://images.unsplash.com/photo-1588348442528-85c6fa3b0440?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwzfHxvcmRlcnxlbnwwfHx8fDE2ODk5NDg1MDF8MA&ixlib=rb-4.0.3&q=85
coverY: -57
---

# 🈁 Tipo conjunto (array)

{% hint style="success" %}
**Vantagem:** o tipo conjunto permite organizar dados de maneira sequencial, algo extremamente poderoso para organizar o código e programar de forma performática economizando recursos de _hardware_.
{% endhint %}

O array é um tipo de dado em JavaScript que permite armazenar múltiplos valores, podendo ser de tipos diversos. É como um conjunto de dados organizados em fila, onde cada elemento tem seu índice que marca sua posição na sequência. É importante lembrar que os índices dos arrays começam a partir do número 0, não do número 1, ou seja, o primeiro elemento está na posição 0, o segundo na posição 1, e assim por diante.

Embora seja comum agrupar dados do mesmo tipo em um array, ele também pode conter uma combinação de strings, numbers e booleans, todos na mesma sequência. A sintaxe para criar um array em JavaScript é simples, utilizando colchetes para delimitar os elementos, e separando cada um deles por vírgulas. Essa forma de representação permite que o JavaScript identifique claramente onde começa e termina cada elemento no array.

Os arrays em JavaScript são bastante versáteis e flexíveis, tornando-se uma estrutura de dados essencial para diversas aplicações. Eles possibilitam o armazenamento e manipulação eficiente de múltiplos valores em uma única variável, facilitando a implementação de algoritmos, iterações e operações que envolvem conjuntos de dados.

```javascript
const amizade = ['Lucas', 'Fernando', 'Maria', 'Carlos', 'Estela'];
```

Para organizar de forma mais legível e amigável as listas em JavaScript, é possível utilizar quebras de linha entre os elementos e incluir uma vírgula após o último. Essa técnica torna a estrutura do array mais clara e facilita a adição de novos elementos posteriormente, pois a vírgula já está previamente inserida. Dessa maneira, o código se torna mais limpo e permite uma melhor visualização dos dados contidos no array, o que é especialmente útil em arrays com muitos elementos ou em situações em que a legibilidade é fundamental para a manutenção do código:

```javascript
const amizade = [
  'Lucas',
  'Fernando',
  'Maria',
  'Carlos',
  'Estela',
];
```

{% hint style="info" %}
Perceba que mesmo dentro do _array_ é uma boa prática respeitar a indentação de código.
{% endhint %}

O acesso aos elementos do _array_ é feito por índice numérico, e sendo assim você pode utilizar os colchetes para obter os valores armazenados com a sintaxe `variavel[numero]`.

```javascript
const amizade = [
    'Lucas',
    'Fernando',
    'Maurício',
    'Luan',
    'Luana',
];

console.log(amizade[0]); //Lucas
console.log(amizade[1]); //Fernando
```

{% hint style="info" %}
Siga [este link](https://coolfee.github.io/#%7B%22code%22%3A%22const%20amizade%20%3D%20%5B%5Cn%20%20%20%20'Lucas'%2C%5Cn%20%20%20%20'Fernando'%2C%5Cn%20%20%20%20'Maur%C3%ADcio'%2C%5Cn%20%20%20%20'Luan'%2C%5Cn%20%20%20%20'Luana'%2C%5Cn%5D%3B%5Cn%5Cnconsole.log\(amizade%5B0%5D\)%3B%20%2F%2FLucas%5Cnconsole.log\(amizade%5B1%5D\)%3B%20%2F%2FFernando%22%2C%22tests%22%3A%22%22%7D) para acessar o código acima_._
{% endhint %}
