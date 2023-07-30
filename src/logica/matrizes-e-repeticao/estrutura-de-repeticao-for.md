---
cover: >-
  https://images.unsplash.com/photo-1621571029036-1573d2b1dc5c?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwxfHxzZXF1ZW5jZXxlbnwwfHx8fDE2OTA3NDMzNDN8MA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🔄 Estrutura de repetição for

{% hint style="success" %}
**Vantagem:** usando estruturas de repetição você pode economizar centenas de milhares de linhas, e até muito mais do que isso, tornando o código belo e de fácil manutenção.
{% endhint %}

A estrutura de repetição "for" em JavaScript é uma forma de executar um bloco de código repetidamente, com base em uma condição específica. É como se você criasse uma contagem regressiva que determina quantas vezes o bloco de código será repetido. Esse tipo de estrutura também é conhecida como _**loop**_ e cada execução do bloco de código é uma **iteração**.

Considere esse _array_ com os nomes de alguns amigos:

```javascript
const amigos = ["João", "Maria", "Carlos", "Ana"];
```

E para mostrar o nome dessas pessoas na tela? Você pode utilizar o índice como viu anteriormente, dessa forma:

```javascript
console.log(amigos[0]); //João
console.log(amigos[1]); //Maria
console.log(amigos[2]); //Carlos
console.log(amigos[3]); //Ana
```

Esta pode ser uma solução aceitável quando o _array_ possui 4 elementos; mas e se fossem milhares de amigos? O código ficaria muito grande com milhares de linhas e de difícil manutenção futura.

É aí que entra a estrutura de repetição, que permite executar quantas vezes for necessário um mesmo bloco de código, variando apenas um **contador** que nesse exemplo é a variável `indice` :

```javascript
const amigos = ["João", "Maria", "Carlos", "Ana"];

for (let indice = 0; indice < amigos.length; indice += 1) {
  console.log(`A pessoa de índice ${indice} é ${amigos[indice]}`);
}
```

A saída fica:

> A pessoa de índice 0 é João\
> A pessoa de índice 1 é Maria\
> A pessoa de índice 2 é Carlos\
> A pessoa de índice 3 é Ana

{% hint style="info" %}
Siga [este link](https://coolfee.github.io/#%7B%22code%22%3A%22const%20amigos%20%3D%20%5B%5C%22Jo%C3%A3o%5C%22%2C%20%5C%22Maria%5C%22%2C%20%5C%22Carlos%5C%22%2C%20%5C%22Ana%5C%22%5D%3B%5Cn%5Cnfor%20\(let%20indice%20%3D%200%3B%20indice%20%3C%20amigos.length%3B%20indice%20%2B%3D%201\)%20%7B%5Cn%20%20console.log\(%60A%20pessoa%20de%20%C3%ADndice%20%24%7Bindice%7D%20%C3%A9%20%24%7Bamigos%5Bindice%5D%7D%60\)%3B%5Cn%7D%22%2C%22tests%22%3A%22%22%7D) para acessar o código acima.
{% endhint %}

Veja como cada parte dessa sintaxe funciona:

1. `let indice = 0`: É criada uma uma variável `indice` que começa com o valor `0`. Essa variável controla a posição do _array_ enquanto percorre seus elementos.
2. `indice < amigos.length`: É a condição que verifica se o bloco de código vai continuar executando ou não. Nesse caso se o valor do índice é **menor** que o comprimento do _array_ `amigos` o bloco de código será executado. Ao utilizar a propriedade `length` que informa quantos elementos existem, o código irá executar 4 vezes uma para cada pessoa, para só depois seguir com o que vem em seguida ao _loop_.
3. `indice += 1`: A cada repetição do _loop_, o código do `console.log` é executado. Isso mostra o nome do amigo da posição `indice` no _array_. Após cada execução do bloco, a variável `indice` é incrementada em 1 (`indice += 1`), ou seja, avançamos para o próximo elemento do _array_ na próxima iteração.

Esse _loop_ continuará até que a condição `indice < amigos.length` seja falsa, ou seja, quando chegar ao final do _array_.

Assim, usando o `for` em conjunto com um _array_ de nomes de amigos, é possível mostrar o nome de cada pessoa de forma simples e eficiente! 🎉
