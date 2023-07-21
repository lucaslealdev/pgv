---
cover: >-
  https://images.unsplash.com/photo-1594392175511-30eca83d51c8?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxyZXR1cm58ZW58MHx8fHwxNjg5MDAyODA5fDA&ixlib=rb-4.0.3&q=85
coverY: -21
---

# ↪ Retorno implícito

{% hint style="success" %}
Vantagem: o uso de retorno implícito permite tornar as funções mais curtas, quando cabível
{% endhint %}

Implícito é aquilo que está lá, mas não precisamos dizer. Dessa forma o retorno implícito é o retorno feito sem colocar o comando `return` propriamente dito.

Isso pode ser feito simplesmente omitindo as chaves `{}` da abertura da função e colocando diretamente o que você deseja retornar após a seta `=>`

### Exemplo usando o gabarito anterior:

{% code lineNumbers="true" %}
```javascript
const areaDoRetangulo = (b, a) => {
  return b*a;
}
// abaixo a versão com o retorno implícito
const areaDoRetangulo2 = (b, a) => b * a;
```
{% endcode %}

Observe que, caso a função tivesse mais de uma linha, não daria para utilizar o retorno implícito. Então os casos em que é possível fazer o retorno implícito são os casos em que a função pode ser escrita usando uma linha apenas dentro do [corpo da função](#user-content-fn-1)[^1].

[^1]: O corpo da função é formado pelas linhas que estão dentro das chaves { }.
