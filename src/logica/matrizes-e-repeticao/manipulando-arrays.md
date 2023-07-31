---
cover: >-
  https://images.unsplash.com/photo-1588348442528-85c6fa3b0440?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwzfHxvcmRlcnxlbnwwfHx8fDE2ODk5NDg1MDF8MA&ixlib=rb-4.0.3&q=85
coverY: -57
---

# 🈁 Manipulando arrays

{% hint style="success" %}
**Vantagem:** uma vez que você souber não apenas criar mas alterar _arrays_, isso irá permitir modificar esses conjuntos para gerar informações.
{% endhint %}

## Adicionando elementos

### Push()

Para adicionar novos elementos a um array, independentemente do tipo dos elementos, você pode utilizar o método push. O método push é usado da seguinte forma: `seuArray.push(novoElemento)`. Isso significa que você pode facilmente inserir qualquer valor, seja número, string, objeto ou até mesmo outro array no final do seu array existente.

```javascript
const conjunto = [];
console.log(`O array conjunto tem o tamanho ${conjunto.length}.`);

conjunto.push(`Fernando`); //adicionando uma string
conjunto.push(42); //adicionando um número
conjunto.push([1, 2, 3]); //adicionando um array dentro do array
console.log(`Agora o array conjunto tem o tamanho ${conjunto.length}.`);
console.log(conjunto);
```

{% hint style="info" %}
Siga [este link](https://esta.la/XL2) para experimentar o código acima.
{% endhint %}

É importante notar que, ao usar o método `push`, você está modificando o _array_ original. Isso significa que o _array_ ao qual você aplicou o `push` será alterado permanentemente após cada chamada do método.

Portanto, o método `push` é uma maneira simples e eficaz de acrescentar elementos ao final de um array, tornando seu código mais flexível e permitindo a manipulação de uma variedade de tipos de dados em uma única estrutura. Compreendendo esse conceito, você estará mais preparado para trabalhar com arrays em JavaScript e desenvolver aplicações mais robustas e dinâmicas.

## Removendo elementos do _array_

Para remover elementos de um _array_ existem muitos métodos, você pode consultar um artigo sobre todos eles [aqui](https://web.archive.org/https://www.geeksforgeeks.org/remove-elements-from-a-javascript-array/).

### Pop()

Para remover o último elemento de um _array_, utilizamos o método `pop`. A sintaxe é `seuArray.pop()`.

```javascript
const amizade = [
    'Lucas',
];
amizade.push('Fernando'); //adiciona Fernando
console.log(amizade.length); //2 (Lucas e Fernando)
amizade.pop(); //remove o último elemento, no caso o Fernando
console.log(amizade.length); //1 (Apenas Lucas)
```

{% hint style="info" %}
Siga [este link](https://coolfee.github.io/#%7B%22code%22%3A%22const%20amizade%20%3D%20%5B%5Cn%20%20%20%20'Lucas'%2C%5Cn%5D%3B%5Cnamizade.push\('Fernando'\)%3B%20%2F%2Fadiciona%20Fernando%5Cnconsole.log\(amizade.length\)%3B%20%2F%2F2%20\(Lucas%20e%20Fernando\)%5Cnamizade.pop\(\)%3B%20%2F%2Fremove%20o%20%C3%BAltimo%20elemento%2C%20no%20caso%20o%20Fernando%5Cnconsole.log\(amizade.length\)%3B%20%2F%2F1%20\(Apenas%20Lucas\)%5Cnconsole.log\(amizade%5B0%5D\)%20%2F%2F%20Lucas%22%2C%22tests%22%3A%22%22%7D) para acessar o código acima_._
{% endhint %}

### Splice()

Para remover um elemento com o índice específico (lembrando que os índices de _array_ começam no zero) você pode utilizar a sintaxe `seuArray.splice(indice, quantidade)` onde `indice` é a posição do elemento onde a remoção se inicia, e `quantidade` é o número de elementos que você deseja remover a partir daquela posição. Comumente é utilizada a quantidade `1` para remover apenas um elemento, mas você pode desejar remover mais de um.

```javascript
const amizade = [
    'Lucas',
];
amizade.push('Fernando'); //adiciona Fernando
console.log(amizade.length); //2 (Lucas e Fernando)
amizade.splice(0, 1); //remove um elemento, partindo do índice 0
console.log(amizade.length); //1 (Apenas Fernando)
console.log(amizade[0]) // Fernando
```

{% hint style="info" %}
Siga [este link](https://coolfee.github.io/#%7B%22code%22%3A%22const%20amizade%20%3D%20%5B%5Cn%20%20%20%20'Lucas'%2C%5Cn%5D%3B%5Cnamizade.push\('Fernando'\)%3B%20%2F%2Fadiciona%20Fernando%5Cnconsole.log\(amizade.length\)%3B%20%2F%2F2%20\(Lucas%20e%20Fernando\)%5Cnamizade.splice\(0%2C%201\)%3B%20%2F%2Fremove%20um%20elemento%2C%20partindo%20do%20%C3%ADndice%200%5Cnconsole.log\(amizade.length\)%3B%20%2F%2F1%20\(Apenas%20Fernando\)%5Cnconsole.log\(amizade%5B0%5D\)%20%2F%2F%20Fernando%22%2C%22tests%22%3A%22%22%7D) para acessar o código acima_._
{% endhint %}
