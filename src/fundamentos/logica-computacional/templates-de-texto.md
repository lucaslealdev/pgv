# 🔳 Templates de texto

{% hint style="success" %}
**Vantagem:** as templates permitem que você crie _strings_ concatenando variáveis de forma muito legível.
{% endhint %}

Com as chamadas _template strings_ ou _template literals_ você pode montar _strings_ incluindo variáveis e constantes de uma forma muito fácil e legível!

A diferença entre uma _template string_ e uma _string_ comum é que ela utiliza crase em vez de aspas, e permite incluir variáveis, constantes e outros códigos JS no meio do texto usando a sintaxe `${}` _(cifrão seguido de chaves)_.

{% code lineNumbers="true" %}
```javascript
const nome = 'Lucas';
const nascimento = 1990;
const anoAtual = new Date().getFullYear();
console.log(`${nome} nasceu em ${nascimento} e tem ${anoAtual - nascimento} anos`);
```
{% endcode %}

{% hint style="info" %}
Siga [este link](https://coolfee.github.io/#\{%22autorun%22:%221%22,%22code%22:%22const%20nome%20=%20'Lucas';\nconst%20nascimento%20=%201990;\nconst%20anoAtual%20=%20new%20Date\(\).getFullYear\(\);\nconsole.log\(%60${nome}%20nasceu%20em%20${nascimento}%20e%20tem%20${anoAtual%20-%20nascimento}%20anos%60\);%22,%22tests%22:%22;%22}) para ver o código acima executando.
{% endhint %}

Essas _templates_ facilitam muito o trabalho, que evita abrir e fechar _strings_ e ficar usando `+` para concatenar!
