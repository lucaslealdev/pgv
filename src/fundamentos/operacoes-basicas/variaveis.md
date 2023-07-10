---
description: >-
  Na matemática temos o X e o Y, que também são variáveis. A boa notícia é que
  na programação você que define os valores das variáveis, em vez de ter que
  descobrir 😉
cover: >-
  https://images.unsplash.com/photo-1527931372109-865f33dff725?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHx2YXJpYWJsZXN8ZW58MHx8fHwxNjg5MDAzMDMyfDA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🧩 Variáveis

{% hint style="success" %}
**Vantagem:** as variáveis são uma facilidade muito grande, pois permitem que você reutilize dados quantas vezes quiser, além de poder dar nome aos dados e assim tornar a intenção do código mais nítida.
{% endhint %}

Variáveis são dados **com nome**. Esse nome é você que inventa e o valor (algum dado) você que determina; esse valor é então guardado na memória temporariamente, para que o seu programa possa utilizar dessa variável até que a execução finalize.

No JS uma variável pode ser definida com o comando `let`. A forma de utilizar é `let nomeDaVariavel`. Observe que os nomes de variável são limitados nos caracteres que podem ter, **não podendo ter acentos ou caracteres especiais (isso inclui `ç`)**; e o primeiro caractere não pode ser um número.

Você também pode criar uma variável já atribuindo um dado a ela, por exemplo com o código `let nome = "Lucas"` .\
Repare que há uma distinção na hora de escrever o que é uma _string_ utilizando aspas, e o que é a variável, que não recebe aspas. Isso permanece sendo uma regra quando você vai utilizar a variável dali em diante, não apenas na hora de criá-la.

No exemplo abaixo uma variável `nome` foi criada já recebendo o valor de `"Lucas"` e é exibida na tela com o `console.log` na segunda linha. A partir daí o seu valor é reatribuido para `"Vitor"` e exibido novamente na tela.

```javascript
let nome = "Lucas";
console.log("Olá " + nome + "! Tudo bem?");
nome = "Vitor";
console.log("Mudamos o valor para " + nome + "! Isso é bem legal!");
```

{% hint style="info" %}
Siga [este link](https://coolfee.github.io/#\{%22autorun%22:%221%22,%22code%22:%22let%20nome%20=%20\\%22Lucas\\%22;\nconsole.log\(\\%22Ol%C3%A1%20\\%22%20+%20nome%20+%20\\%22!%20Tudo%20bem?\\%22\);\nnome%20=%20\\%22Vitor\\%22;\nconsole.log\(\\%22Mudamos%20o%20valor%20para%20\\%22%20+%20nome%20+%20\\%22!%20Isso%20%C3%A9%20bem%20legal!\\%22\);%22,%22tests%22:%22;%22}) para acessar o código acima_._
{% endhint %}

### Erros comuns

Como o código é executado linha por linha, é importante notar que se você tentar utilizar uma variável antes de ela existir, isso causa um erro. Esse exemplo abaixo é uma forma de como você **não pode** utilizar variáveis:

{% hint style="danger" %}
```javascript
console.log(nome);
let nome = "Lucas";
```
{% endhint %}

O erro exibido no console será _<mark style="color:red;">`Cannot access 'nome' before initialization`</mark>_, que traduzindo com o tradutor automático fica _<mark style="color:red;">`Não é possível acessar 'nome' antes da inicialização`</mark>_.

Esse erro diz justamente o que foi feito de errado, tentar acessar a variável nome antes da sua inicialização. Caso a variável sequer seja definida no código, isso muda um pouco.

{% hint style="danger" %}
```javascript
console.log(nome);
```
{% endhint %}

Nesse caso o erro exibido será _<mark style="color:red;">`nome is not defined`</mark>_. De fato, nome realmente é uma variável que não foi definida.\
O interpretador[^1] do JavaScript tenta sempre te mostrar erros personalizados da forma mais nítida possível, para que você consiga deduzir o que fez de errado. A limitação das linguagens de programação é não saber o que você está tentando fazer (já que elas em geral não contam com inteligência artificial), e por isso as mensagens não tem como serem mais nítidas ainda.

{% hint style="warning" %}
Importante: você consegue criar variáveis sem a utilização do `let`, colocando apenas <mark style="color:orange;">`variavel = 3;`</mark> ou usando "var" em vez do let, <mark style="color:orange;">`var variavel = 3;`</mark>. Porém você não deveria fazer isso, pois existem diferenças práticas no resultado, que você aprenderá nos capítulos mais avançados deste guia. Por agora, podemos resumir que é uma boa prática de programação utilizar o `let` na hora de criar a variável.
{% endhint %}

[^1]: Interpretador é como chamamos o software que executa, linha por linha, o código que escrevemos.
