# 5 Tipo número (number)

{% hint style="success" %}
**Vantagem:** quando você consegue manipular o tipo número, isso permite que você faça cálculos.

**Racional:** saber como utilizar números também vai permitir você aprender coisas mais avançadas mais adiante, que necessitam do entendimento do dado _number_.
{% endhint %}

O tipo _number_ inclui quase todos os tipos de número que a matemática nos oferece. Temos números inteiros como `37`, números quebrados (reais) como `3.14`, números negativos como `-34.14`, o número infinito `infinity`, e até o número impossível como `NaN`. Diferente do tipo _string_, os números não são representados com aspas.

{% hint style="warning" %}
O NaN (_not a number_/não é número) é a representação do JavaScript do que não é um número válido e por isso normalmente é entendido como um erro. Pode ser que você já tenha vivido o _NaN_ na sua vida ao tentar na calculadora calcular `0/0`, o que dá erro mesmo em calculadoras simples pois não é possível dividir zero por zero. No JavaScript `0/0` resulta em `NaN`.
{% endhint %}

Com o dado do tipo _number_ você pode utilizar os operadores matemáticos para fazer contas. Os operadores básicos são `+`, `-`, `*` e `/`, respectivamente soma, subtração, multiplicação e divisão.

Importante notar que como o operador de soma `+` é o mesmo operador utilizado para concatenar _strings_, a ordem de como você utiliza _strings_ e números vai determinar como o JS (_JavaScript_) entende o que você quer que aconteça, se é concatenação ou soma.

<pre class="language-javascript"><code class="lang-javascript"><strong>console.success(13 + 3);
</strong>console.success(12 / 3);
console.success(13 + 3 + " é o resultado da soma de 13 com 3");
console.success("Ao dividir 12 por 3 temos: " + 12 / 3);
console.error("Ao iniciar com string, o + deixa de significar soma: " + 12 + 3);
</code></pre>

{% hint style="info" %}
Siga [este link](https://coolfee.github.io/#\{%22autorun%22:%221%22,%22code%22:%22console.success\(13%20+%203\);\nconsole.success\(12%20/%203\);\nconsole.success\(13%20+%203%20+%20\\%22%20%C3%A9%20o%20resultado%20da%20soma%20de%2013%20com%203\\%22\);\nconsole.success\(\\%22Ao%20dividir%2012%20por%203%20temos:%20\\%22%20+%2012%20/%203\);\nconsole.error\(\\%22Ao%20iniciar%20com%20string,%20o%20+%20deixa%20de%20significar%20soma:%20\\%22%20+%2012%20+%203\);%22,%22tests%22:%22;%22}) para acessar o código acima_._
{% endhint %}
