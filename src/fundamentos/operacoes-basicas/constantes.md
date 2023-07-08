# 🏛 Constantes

{% hint style="success" %}
**Vantagem:** criar constantes garante que no seu código hoje e no futuro, os valores não serão reatribuidos, diferente das variáveis.
{% endhint %}

Constantes são similares às variáveis que você já aprendeu. Só que elas são **imutáveis**, então caso o código tente fazer uma reatribuição `nome = 'Lucas';` isso geraria um erro.

{% hint style="danger" %}
{% code lineNumbers="true" %}
```javascript
const nome = 'Lucas';
nome = 'Vitor';
```
{% endcode %}
{% endhint %}

No exemplo acima, a linha 2 gera um erro, pois está tentando reatribuir uma constante.

### Mas, por quê?

Você deve estar se perguntando qual a grande vantagem de utilizar constantes, já que as variáveis declaradas com `let` funcionam também e são mais vantajosas pois permitem mudar o valor posteriormente.

A razão é aproveitar essa desvantagem da constante como uma mensagem para a pessoa programadora que está mexendo no código, que pode ser até você. Quando você se depara com uma constante, você sabe com certeza que aquele valor não será reatribuido! Então há um significado semântico[^1] para quem lê o código.\
Por isso, por boa prática, todo dado deve ser criado como `const`, e apenas mediante a necessidade da reatribuição colocamos como `let`.

[^1]: A _semântica_ é a área da linguística que estuda o significado e a sua relação com o significante.
