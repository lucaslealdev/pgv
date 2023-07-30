---
cover: >-
  https://images.unsplash.com/photo-1629706168156-d2d0558c972e?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwxfHxwYXJhbWV0ZXJzfGVufDB8fHx8MTY4OTAwMjg0MHww&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🚜 Funções com parâmetros

{% hint style="success" %}
**Vantagem:** quando você cria uma função que recebe um parâmetro isso permite reutilizá-la em cenários mais diversos, que variam conforme o parâmetro.
{% endhint %}

As funções em JavaScript também podem receber parâmetros, que são como variáveis especiais! A grande diferença é que os nomes desses parâmetros são determinados dentro dos parênteses da função, e não usam a palavra-chave "let" para declará-los.

Quando você define uma função, deve colocar parênteses no início da declaração. Dentro desses parênteses, você inclui os nomes dos parâmetros separados por vírgulas. Esses parâmetros funcionam como variáveis que podem ser usadas dentro da função.

Quando você chama a função e passa os valores entre os parênteses, esses valores são atribuídos aos parâmetros na ordem em que são fornecidos. Assim, os parâmetros permitem que a função receba informações externas para trabalhar com elas.

Essa é uma funcionalidade poderosa porque torna as funções mais flexíveis e reutilizáveis. Podemos criar uma função genérica que aceita diferentes valores por meio de parâmetros, o que nos permite executar a mesma lógica em situações diferentes. Compreender como usar e trabalhar com parâmetros é fundamental para tirar o máximo proveito das funções em JavaScript!

{% code lineNumbers="true" %}
```javascript
const imc = (nome, peso, altura) => {
  const calculo = (peso / (altura * altura)).toFixed(2);
  console.log(`O IMC de ${nome} é ${calculo} kg/m2.`);
};

imc('Vitor', 80, 1.79); //console: O IMC de Vitor é 24.97 kg/m2.
imc('João', 75, 1.71); //console: O IMC de João é 25.65 kg/m2.
```
{% endcode %}

{% hint style="info" %}
Siga [este link](https://esta.la/PpV) para ver o código acima executando.\
Nota: Este código utiliza a função `toFixed()` ([documentação](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global\_Objects/Number/toFixed)) que é utilizada na sintaxe `algumNumero.toFixed(casasDecimais)` para reduzir o número de casas decimais, já que comumente a divisão gera um número maior de casas devido à precisão de números reais que o JavaScript oferece. [Aqui](https://web.archive.org/web/https://pt.stackoverflow.com/questions/14728/realiza%C3%A7%C3%A3o-de-contas-de-ponto-flutuante-em-javascript-com-precis%C3%A3o-absoluta/14781) no stackoverflow há uma explicação matemática detalhada do racional por trás disso, mas não é necessário saber disso com detalhe.
{% endhint %}

Receber parâmetros em funções é incrível, pois permite reutilizar essa função muito melhor, já que os dados não são mais fixos dentro dela.
