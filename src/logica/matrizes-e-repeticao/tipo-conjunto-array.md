---
cover: >-
  https://images.unsplash.com/photo-1588348442528-85c6fa3b0440?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwzfHxvcmRlcnxlbnwwfHx8fDE2ODk5NDg1MDF8MA&ixlib=rb-4.0.3&q=85
coverY: -57
---

# 🈁 Tipo conjunto (array)

O tipo de dado conjunto, chamado de _array_ (do inglês _variedade_), permite armazenar não apenas um dado, mas vários e de tipos diversos. O mais comum é termos agrupamentos de dados do mesmo tipo, mas nada impede de haver um _array_ que possui _strings, numbers_ e _boolean_ tudo na mesma sequência.

Esse tipo de dado é organizado sempre em **fila**, um elemento atrás do outro, cada um tendo seu índice que demarca sua ordem. É importante sempre lembrar que esse índice começa no número 0, não no número 1, por isso o primeiro elemento de um _array_ está na posição 0, o segundo na posição 1, e assim por diante.

A sintaxe de criação de _array_ é utilizando o colchete para receber os elementos, e cada um é separado por vírgula do próximo. Assim, o JavaScript consegue identificar onde começa e termina cada elemento.

```javascript
const amizade = ['Lucas', 'Fernando', 'Maria', 'Carlos', 'Estela'];
```

Para organizar melhor a lista, o JavaScript permite também que sejam utilizadas quebras de linha **entre os elementos** e incluir uma vírgula após o último, o que facilita a inclusão de mais elementos ali posteriormente já que a vírgula já está colocada:

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

