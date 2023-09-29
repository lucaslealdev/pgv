# Clonando um repositório

Embora utilizemos o nome **clone**, ele não é exatamente uma cópia no sentido que costumamos utilizar a palavra clone. Quando você clona um repositório, você está fazendo o _download_ dele para o seu computador, e não criando uma cópia visível na internet como pode dar a entender o uso da expressão "clone".

O comando para clonar um repositório remoto é o `git clone`, e ele recebe um parâmetro que é o caminho do repositório a ser clonado (como se fosse um link).

{% hint style="warning" %}
Tenha atenção ao _clonar_ um repositório, pois não é esperado que se faça um clone de um repositório **dentro** de uma pasta que já seja um repositório. Até existem situações específicas em que isso é feito, mas elas são incomuns. No uso do dia-a-dia, clonar um repositório dentro de outro repositório pode causar problemas.
{% endhint %}

Para fazer pela primeira vez, iremos clonar o repositório `lucaslealdev/repositorio_teste`.

1. Acesse o repositório pelo navegador, [aqui](https://github.com/lucaslealdev/repositorio\_teste).
2. Clique no botão verde com o texto `<> Code`.
3. Selecione a opção SSH.
4. Ao lado da caixa de texto que começa com `git@github.com:lucasleal...`, há um botão para copiar esse link SSH do repositório.
5. No terminal, utilize o comando `git clone git@github.com:lucasleal(...)` colando o link completo.

Após esse comando ser feito, surgirá uma nova pasta chamada `repositorio_teste` dentro da pasta onde você se encontra no terminal. Lá está o seu repositório! Se listando os arquivos dessa pasta você encontrar o arquivo `README.md`, deu tudo certo!
