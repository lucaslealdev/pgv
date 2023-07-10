---
cover: >-
  https://images.unsplash.com/photo-1550376026-7375b92bb318?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwxfHxvcmdhbml6YXRpb258ZW58MHx8fHwxNjg5MDAyODc2fDA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 😎 Indentação

Anteriormente ao aprender a criar uma função, você deve ter reparado que o nosso exemplo incluía um tipo de recuo do texto; um espaço entre o começo da linha e o código, quando dentro da função. Algo parecido com isso:

{% code lineNumbers="true" %}
```javascript
const funcaozinha = () => {
  console.log('Aqui foi dado um espacinho no começo da linha');
};
```
{% endcode %}

O nome dessa organização do código é **indentação** e existe para que você (e outras pessoas) ao olhar o código possa saber onde começa e onde termina esse "bloco" do código imediatamente, seja esse bloco uma função ou outras estruturas que aprenderá mais à frente.

Na função `funcaozinha` é sabido que a linha 2 é o corpo da função e mesmo sem a indentação isso seria nítido, pois é uma função bem pequena com uma linha apenas. No entanto ao criar funções maiores e mais complexas, essa visibilidade dos blocos de código através do recuo será muito útil. Esse recuo pode ser feito utilizando a tecla **tab** do teclado.
