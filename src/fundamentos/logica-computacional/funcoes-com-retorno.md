---
cover: >-
  https://images.unsplash.com/photo-1594392175511-30eca83d51c8?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxyZXR1cm58ZW58MHx8fHwxNjg5MDAyODA5fDA&ixlib=rb-4.0.3&q=85
coverY: -21
---

# ↪ Funções com retorno

{% hint style="success" %}
Vantagem: o _retorno_ da função é uma de suas maiores vantagens, pois permite que ela devolva dados para onde a função foi chamada.
{% endhint %}

O retorno dentro da função é o que permite que você expanda ainda mais a reutilização delas. Além de chamar a função e colocar os parâmetros, você pode utilizar o dado que ela gera através do retorno!

Assim conseguimos manipular esses dados e misturá-los com outros, exibí-los juntos e tudo que sua imaginação permitir.

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
imc('João', 76, 1.71); //Console: O IMC de João é 25.99 kg/m2.
idade('João', 1995); //Console: João tem 28 anos.
```
{% endcode %}

{% hint style="info" %}
### Saída:

O IMC de João é 25.99 kg/m2.

João tem 28 anos.
{% endhint %}

Observe que, sem usar o retorno, você não consegue **interceptar** o que cada função calculou e isso impede que você crie uma mensagem mais interessante, como por exemplo `O IMC de João é 25.99 kg/m2 e ele possui 28 anos.` Essa mensagem **mistura** as duas funções, então só é possível produzí-la com o uso do retorno.

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

Observe que com o retorno você pode **usar** o resultado do que a função fez, em vez de ficar limitado a manipular o dado apenas internamente na função. De repente, o resultado consegue **sair** dela.

É importante notar também a diferença do `return` e do `console.log`, que não são a mesma coisa e não faz sentido misturá-los na mesma linha. O `return` permite sair da função com o dado que vem adiante, enquanto que o `console.log` serve pra mostrar dados no console.

Agora, vamos para o primeiro exercício da seção!
