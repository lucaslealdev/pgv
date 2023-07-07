# 🧠 Utilizando IAs para entender erros



{% hint style="success" %}
**Vantagem:** se você souber utilizar bem a inteligência artificial, pode sair na frente resolvendo problemas complexos de forma mais rápida.
{% endhint %}

O chatGPT é uma inteligência artificial baseada em conversa, ou seja, você pode perguntar o que quiser e a IA vai te responder. Isso inclui perguntas sobre programação!

Se você perguntar sobre um erro de variável não inicializada, veja o que ela responde:

> O código abaixo tem um erro, consegue me ajudar a resolver?\
> console.log(nome);\
> let nome = "Lucas";

> Certamente posso ajudar! O erro no código é causado pelo fato de você estar tentando acessar a variável `nome` antes de declará-la.
>
> Quando você declara uma variável utilizando a palavra-chave `let`, é importante que a declaração ocorra antes de qualquer tentativa de acesso ou uso dessa variável no código. No seu exemplo, você está tentando acessar `nome` antes de declará-la, o que causa um erro.
>
> Para corrigir o código, você pode simplesmente mover a declaração da variável `nome` para antes do `console.log(nome)`, desta forma:
>
> ```javascript
> let nome = "Lucas";
> console.log(nome);
> ```
>
> Dessa forma, a variável `nome` será declarada antes de ser acessada, e o código irá funcionar corretamente, exibindo "Lucas" no console.

Veja que impressionante! A inteligência artificial prontamente entendeu o código, sabendo até qual foi o erro que deu, não foi preciso nem dizer.

Naturalmente que a IA pode não ter todas as respostas, e pode também responder errado. Mas é uma ajuda muito boa no avanço do entendimento da programação e você deve com certeza utilizá-la.
