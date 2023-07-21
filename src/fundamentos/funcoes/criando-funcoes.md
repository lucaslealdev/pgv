---
description: >-
  Quase todas linguagens de programação possuem o recurso de criar funções, que
  são trechos de código organizados com começo, meio e fim.
cover: >-
  https://images.unsplash.com/photo-1613178594694-5f96ae9b5bb0?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw0fHxmdW5jdGlvbnxlbnwwfHx8fDE2ODkwMDI5MTZ8MA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🔧 Criando funções

{% hint style="success" %}
**Vantagem**: a vantagem de você saber como usar funções é poder reutilizar código infinitas vezes, inclusive ao criar novos programas, usando parte do código que você já acumulou durante seu aprendizado. Digitar menos, programar mais.
{% endhint %}

As funções são pedaços de código, o que lembra muito o processo de uma linha de produção de fábrica. Cada trecho da linha de produção recebe um produto semi-acabado, trabalha nesse produto, e no fim devolve um produto um pouco mais acabado; até que no fim temos o produto finalizado. Nessa analogia, cada trecho da linha de produção é uma função específica.

O nome _função_ fala exatamente sobre isso! A função deve ter apenas um único objetivo (ou o mais próximo disso possível) e deve permitir reutilização. Em uma linha de produção de carros, o time que coloca os pneus tem apenas um objetivo e pode cumprir esse objetivo para uma infinidade de carros diferentes, permitindo a **reutilização** dos seus aparatos.

No JavaScript, para criar funções é preciso uma organização específica de comandos, que é assim:

```javascript
const nomeDaFuncao = () => {
    //o código da função vem aqui
};
```

Isso é a **sintaxe** de como definir funções. Ou seja, você cria a constante com o nome que deseja para a função, e no valor coloca a função em si. A função precisa começar com parênteses, ter uma setinha (_arrow_) e depois as chaves `{}`. Dentro dessas chaves, você coloca o código que a função vai executar. Utilizamos constantes pois seria muito estranho uma função ser reatribuída, causando confusão no entendimento do código. A constante não pode ser reatribuída, por isso garante esse comportamento.

Sempre que a função do código abaixo for chamada, ela exibirá a mensagem `"Bom dia!"`. Isso pode ser testado chamando a função algumas vezes. Para chamar uma função você chama pelo seu nome seguido de parênteses, e você já viu isso antes! O `console.log` utilizado várias vezes anteriormente é uma função que já vem incluída no JavaScript.

<pre class="language-javascript" data-line-numbers><code class="lang-javascript"><strong>const bomDia = () => {
</strong>    console.log("Bom dia!");
};
console.log("Hoje é um bom dia!");
bomDia();
console.log("Que legal!");
bomDia();
</code></pre>

{% hint style="info" %}
Siga [este link](https://esta.la/2mL) para acessar o código acima_._
{% endhint %}

Observe que a ordem do programa agora não é **exatamente** linha-após-linha. Mesmo o código que exibe a mensagem de bom dia estando na linha 2, ele só executa quando chamamos a função na linha 5, e depois continua normalmente indo direto para a linha 6.

Isso acontece por causa da capacidade da função de ser chamada, fazer o que deve fazer, e depois voltar para o código na linha seguinte de onde a função foi chamada. É viagem no tempo, só que no código.
