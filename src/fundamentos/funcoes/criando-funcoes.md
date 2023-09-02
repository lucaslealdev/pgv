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

As funções são como os diferentes estágios em uma linha de produção de fábrica, onde cada etapa recebe um produto semi-acabado, trabalha nele e, no final, entrega um produto mais refinado. Essa analogia nos ajuda a entender que cada parte da linha de produção representa uma função específica.

O próprio termo "função" reflete essa ideia! Cada função deve ter um único objetivo bem definido (ou o mais próximo disso possível) e ser projetada para permitir sua reutilização em várias situações. Imagine uma linha de produção de carros: o time responsável por colocar os pneus tem um único objetivo, que pode ser aplicado a uma infinidade de carros diferentes, tornando seus equipamentos facilmente reutilizáveis.

Ao criar funções com um propósito claro e reutilizável, podemos simplificar nossos códigos, tornando-os mais eficientes, organizados e fáceis de manter. Assim, assim como uma linha de produção bem estruturada otimiza a fabricação de produtos, funções bem projetadas aprimoram a criação de soluções na programação. Você irá explorar essa abordagem e aproveitar ao máximo a versatilidade e eficácia das funções em seus projetos!

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
