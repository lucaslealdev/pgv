# 🧪 Operações com variáveis

{% hint style="success" %}
**Vantagem:** como as variáveis podem ser reutilizadas, é muito conveniente para reaproveitamento de código e repetição de operações.
{% endhint %}

Anteriormente você viu que pode estabelecer dados em _string_ para as variáveis. Mas também consegue fazer isso com números e utilizá-los nos cálculos.\
O exemplo de código abaixo exibe o tempo que o carro de Lucas levaria para percorrer distâncias variadas com uma velocidade fixa, armazenada na variável `velocidade`.

{% hint style="info" %}
Dica: como o código abaixo inicia com uma _string_, o operador + seria entendido como concatenação, não é? **Não**. Aqui, como há uma **divisão**, e a divisão ocorre antes da soma pela regra da precedência matemática, esse problema está resolvido automaticamente no entendimento do JavaScript.\
**No entanto, para aumentar a nitidez das operações, a conta foi colocada entre parênteses, que seria a solução caso a conta fosse de soma.**
{% endhint %}

```javascript
let velocidade = 80;
let nome = "Lucas";
console.log("O carro de " + nome + " percorreria 80Km em " + (80 / velocidade) + "h");
console.log("O carro de " + nome + " percorreria 180Km em " + (180 / velocidade) + "h");
console.log("O carro de " + nome + " percorreria 1745Km em " + (1745 / velocidade) + "h");
```

{% hint style="info" %}
Siga [este link](https://esta.la/e3Y) para acessar o código acima_._
{% endhint %}

Veja que a reutilização da variável permite que você troque a velocidade do carro de Lucas apenas uma vez no código, na linha 1, alterando o resultado de todos os `console.log` de uma vez só.
