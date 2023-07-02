---
description: >-
  Na matemática temos o X e o Y, que também são variáveis. A vantagem é que na
  programação você que define os valores das variáveis, em vez de ter que
  descobrir 😉
---

# 🧩 Variáveis

{% hint style="success" %}
**Vantagem:** as variáveis são uma facilidade muito grande, pois permitem que você reutilize dados quantas vezes quiser, além de poder dar nome aos dados e assim tornar a intenção do código mais nítida.
{% endhint %}

No JS uma variável pode ser definida com o comando `let`. A forma de utilizar é `let nomeDaVariavel`.\
Você também pode criar uma variável já atribuindo um dado a ela, por exemplo com o código `let nome = "Lucas"` .\
Repare que há uma distinção na hora de escrever o que é uma _string_ utilizando aspas, e o que é a variável, que não recebe aspas. Isso permanece sendo uma regra quando você vai utilizar a variável dali em diante, não apenas na hora de criá-la.

```javascript
let nome = "Lucas";
console.log("Olá " + nome + "! Tudo bem?");
```

{% hint style="info" %}
Siga [este link](https://coolfee.github.io/#\{%22autorun%22:%221%22,%22code%22:%22let%20nome%20=%20\\%22Lucas\\%22;\nconsole.log\(\\%22Ol%C3%A1%20\\%22%20+%20nome%20+%20\\%22!%20Tudo%20bem?\\%22\);%22,%22tests%22:%22;%22}) para acessar o código acima_._
{% endhint %}

Como o código é executado linha por linha, é importante notar que tentar utilizar uma variável antes de ela existir irá causar um erro. Esse exemplo abaixo é uma forma de como você não pode utilizar variáveis:

{% hint style="danger" %}
```javascript
console.log(nome);
let nome = "Lucas";
```
{% endhint %}

**Em construção**
