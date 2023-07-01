# 🔤 Tipo texto (string)

{% hint style="success" %}
**Vantagem:** saber manipular texto é imprescindível para programação pois é através do texto que você vai se comunicar com o usuário e vice-versa.
{% endhint %}

A _string,_ do inglês _linha_ é um tipo de dado que armazena texto, tendo esse nome por se tratar de uma sequência de caracteres. Por exemplo, `"Aprender"` é uma _string_ de comprimento 8 (pois tem oito letras), cujos caracteres estão ligados por uma linha imaginária (daí o nome _string_) e são respectivamente A-p-r-e-n-d-e-r.

Repare que, no JavaScript, a _string_ vem sempre entre aspas `""` ou apóstrofos `''` e não há diferença prática entre aspas e apóstrofos na formação de _strings._ No entanto é comum que visando qualidade os times de programadores combinem um padrão a ser seguido de utilizar um em detrimento do outro.

As _strings_ podem ser **concatenadas**, o que significa colar umas às outras em sequência, formando uma nova _string_ com duas ou mais partes. Isso vai ser muito útil conforme você precisar juntar dados inseridos pelo usuário e dados que são do sistema. Uma mensagem de bem-vindo que inclua o nome do usuário é um exemplo de concatenação.

```javascript
console.log("Essa é uma string criada com aspas");
console.log("Essa é uma string criada com apóstrofos");
console.log("Olá " + 'João' + '! Seja bem-vindo!');
```

{% hint style="info" %}
Siga [este link](https://coolfee.github.io/#\{%22autorun%22:%221%22,%22code%22:%22console.log\(\\%22Essa%20%C3%A9%20uma%20string%20criada%20com%20aspas\\%22\);\nconsole.log\(\\%22Essa%20%C3%A9%20uma%20string%20criada%20com%20ap%C3%B3strofos\\%22\);\nconsole.log\(\\%22Ol%C3%A1%20\\%22%20+%20'Jo%C3%A3o'%20+%20'!%20Seja%20bem-vindo!'\);%22,%22tests%22:%22;%22}) para acessar o código acima_._
{% endhint %}
