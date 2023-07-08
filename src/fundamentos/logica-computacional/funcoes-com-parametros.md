# 🔳 Funções com parâmetros

{% hint style="success" %}
**Vantagem:** quando você cria uma função que recebe um parâmetro isso permite reutilizá-la em cenários mais diversos, que variam conforme o parâmetro.
{% endhint %}

As funções também podem receber parâmetros, que são como variáveis porém seus nomes são determinados dentro do parênteses da função.

{% code lineNumbers="true" %}
```javascript
const imc = (nome, peso, altura) => {
  const calculo = (peso / (altura * altura)).toFixed(2);
  console.log(`O IMC de ${nome} é ${calculo} kg/m2.`);
};

imc('Vitor', 80, 1.79); //console: O IMC de Vitor é 24.97 kg/m2.
```
{% endcode %}

{% hint style="info" %}
Siga [este link](https://esta.la/wxQ) para ver o código acima executando.
{% endhint %}

Essas _templates_ facilitam muito o trabalho, que evita abrir e fechar _strings_ e ficar usando `+` para concatenar!
