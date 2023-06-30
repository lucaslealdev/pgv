---
description: >-
  Olá mundo é uma frase muito conhecida entre desenvolvedores por ser um padrão
  da primeira coisa que se faz em qualquer linguagem de programação: pedir para
  o computador escrever algo na tela.
---

# 🌎 Olá, mundo! (console.log)

{% hint style="info" %}
**Racional**: A vantagem de saber como exibir informações de registro é poder analisar como o código está funcionando; e nesse momento utilizaremos isso para realizar operações básicas de modo que possamos entender como o JavaScript opera, nessa e nas próximas lições.
{% endhint %}

Um método muito utilizado e que serve justamente para exibir um dado ou informação é o `console.log` (documentação do método [aqui](https://developer.mozilla.org/en-US/docs/Web/API/console/log)). Nesse comando, _console_ é onde vamos mostrar a informação e _log_ é do inglês _registro,_ já que o comando serve para fazer um registro temporário de informações na tela. Veja um exemplo de uso:

{% code title="exemplo-console.log.js" lineNumbers="true" fullWidth="false" %}
```javascript
console.log("Olá, mundo! Eu estou vivo!");
```
{% endcode %}

O comando acima tem como resultado exibir a frase  [<mark style="background-color:green;">Olá, mundo! Eu estou vivo!</mark> ](#user-content-fn-1)[^1] para o usuário.\
Siga [esse link](https://coolfee.github.io/#\{%22autorun%22:%221%22,%22code%22:%22\(\(\)%20=%3E%20{\n%20%20//aqui%20vem%20o%20c%C3%B3digo\n%20%20console.log\(\\%22Ol%C3%A1,%20mundo!%20Eu%20estou%20vivo!\\%22\);\n}\)\(\);%22,%22tests%22:%22;%22}) para ver esse código executando no navegador.

{% hint style="info" %}
**Para experimentar**: Uma vez na plataforma, altere o conteúdo da mensagem e clique no botão _Run (ctrl/cmd + s)_ para ver que o texto exibido à direita se modifica.
{% endhint %}

O _log_ é uma forma rudimentar de conversar com o usuário, e abre um mundo enorme de coisas que podemos experimentar. Como faríamos por exemplo para mostrar números em vez de texto? Podemos colocar números dentro das aspas? Que diferença faz? Veremos isso na nossa próxima lição.

[^1]: Importante: veja que as aspas fazem parte da forma de escrever um texto que não é um comando, mas um texto literalmente dizendo. Por isso, as aspas não aparecem na tela.
