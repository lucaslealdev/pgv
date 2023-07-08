# ↪ Funções com retorno

{% hint style="success" %}
Vantagem: o _retorno_ da função é uma de suas maiores vantagens, pois permite que ela devolva dados para onde a função foi chamada.
{% endhint %}

O retorno dentro da função é o que permite que você expanda ainda mais a reutilização delas. Além de chamar a função, você pode utilizar ela como um dado através do retorno!

Assim conseguimos manipular esses dados e misturá-los com outros, exibí-los juntos e tudo que sua imaginação permitir. Veja exemplos adiante.

### Exemplo de uso com função comum sem retorno:

{% code lineNumbers="true" %}
```javascript
const imc = (nome, peso, altura) => {
  const calculo = (peso / (altura * altura)).toFixed(2);
  console.log(`O IMC de ${nome} é ${calculo} kg/m2.`);
};
const idade = (nome, nascimento) => {
  console.log(`${nome} tem ${new Date().getFullYear() - nascimento} anos.`);
};
imc('João', 76, 1.71);
idade('João', 1995);
```
{% endcode %}

Saída:

> O IMC de João é 25.99 kg/m2.
>
> João tem 28 anos.

Observe que, sem usar o retorno, você não consegue **interceptar** o que cada função calculou e isso impossibilita criar uma mensagem mais interessante como por exemplo `O IMC de João é 25.99 kg/m2 e ele possui 28 anos.` Essa mensagem mistura as duas funções, então só conseguimos produzí-la com o uso do retorno.

### Exemplo de uso com função que tem retorno:

{% code lineNumbers="true" %}
```javascript
const imc = (peso, altura) => {
  const calculo = (peso / (altura * altura)).toFixed(2);
  return calculo;
};
const idade = (nascimento) => {
  return new Date().getFullYear() - nascimento;
};

console.log(`O IMC de João é ${imc(76, 1.71)} e ele tem ${idade(1995)} anos de idade.`);
```
{% endcode %}

{% hint style="info" %}
Siga [este link](https://esta.la/9GX) para ver o código acima.
{% endhint %}

Observe que com o retorno você pode **usar** o resultado do que a função fez, em vez do uso ficar limitado a manipular o dado apenas internamente.

É importante notar também a diferença do `return` e do `console.log`, que não são a mesma coisa e não faz sentido misturá-los na mesma linha pois a função `console.log` **mostra** algo no console, mas ela não **retorna** nada.
