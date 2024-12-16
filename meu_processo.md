# Meu processo

Para a entrega satisfatória do projeto, foi necessário mudanças nos passos para confirmar a extração de dados usando o SETOOLKIT. Detalharei em seguida como cheguei à extração dos dados por meio da ferrament.

## Passo 1

Após executar os simples passos expostos no README, mesmo com a conexão aberta e a página acessível em outra máquina, o retorno da conexão não entrega email e senha inseridas na página de phishing. Apenas códigos como pode ser visto abaixo.

![erro](/erro.png)

Ao pesquisar as mensagens para encontrar uma possível solução, mesmo encontrando o problema relatado por outras pessoas, não encontrei nada que pudesse resolver a questão.

Sendo assim tentei descobrir se era algum problema na versão que estava usando. Fiz as atualizações na tela inicial do SETOOLKIT, mas a falta de feedback do programa me deixaram em dúvida se algum tipo de atualização foi realmente efetuada.

Para tentar garantir que estava rodando uma versão mais recente baixei a versão mais atualizada do Kali Linux no site oficial, mas obtive o mesmo retorno anterior.

Como veremos abaixo, **o passo 1 não foi importante para resolvermos o problema.**

## Passo 2

Já com a suspeita de que o problema poderia estar no site, tentei usar outros sites. Tentei os seguintes sites:
- Instagram
- Magazine Luiza
- Amazon

Dessa vez o problema foi a clonagem da página. Ou a clonagem não funcionava corretamente, apresentando uma página quebrada e/ou mal configurada ou o programa retornava erro de impossibilidade de clonar a página enviada.

## Passo 3

Dessa vez busquei usar as outras opções que o SETOOLKIT oferece:

- Tipo de ataque: ``` Social-Engineering Attacks ```
- Vetor de ataque: ``` Web Site Attack Vectors ```
- Método de ataque: ```Credential Harvester Attack Method ```
- Método de ataque: ``` Web Templates ```
- Template: ``` Google ```

Após selecionar essas opções a página foi exibida corretamente e então tive o primeiro retorno bem-sucedido:

![template_google](/template_google.png)

## Passo 4

Para conseguir me manter mais fiel à proposta inicial de clonar a página do Facebook, consegui descobrir como contornar isso e confirmei que a Meta usou códigos anti-phishing para impedir o usos de ferramentas como o SETOOLKIT. Dessa maneira os passos dentro do programa seguem:

- Tipo de ataque: ``` Social-Engineering Attacks ```
- Vetor de ataque: ``` Web Site Attack Vectors ```
- Método de ataque: ```Credential Harvester Attack Method ```
- Método de ataque: ``` Custom Template ```
- Caminho: ``` "caminho do arquivo dentro do Kali ```

# Como criar o arquivo do Facebook

