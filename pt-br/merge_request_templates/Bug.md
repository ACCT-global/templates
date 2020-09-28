# Bug

## Fix Type:
- _Nesta sessão deverá ser explicitado se esse bugfix é uma correção simples, um bugfix que acarretará na mudança do comportamento de alguma funcionalidade parcialmente ou totalmente ou se alguma informação referente a documentação ficará obsoleta e precisará ser atualizada._

- [x] - Minor Bugfix.

- [ ] - Bugfix with Breaking Change.

- [ ] - Change requires a Documentation update.

_**OBS: Deletar checkboxes que não são se aplicam ao Merge Request.**_

## Overview:

_Aqui vai uma explicação do bug, porque é um bug, comportamento atual e comportamento esperado, além de um link direto para a issue a qual o MR está ligado_

>Ex:
> - Comportamento atual: Botão de adicionar mais 1 item ao carrinho de compras não dá nenhum feedback que a ação ocorreu ao ser clicado.
> - Comportamento esperado: Botão deve entrar em um estado suspenso tanto para dar um feedback para o usuário quanto para impedir adições subsequentes antes que a mudança de quantidade ocorra.
- ### **Related Issues:**
  - [#12](https://google.com.br)
  - [#25](https://google.com.br)
  - [#99](https://google.com.br)

## Reproduction Steps:

_Passo a passo para reprodução do bug, se for reproduzível e em qual ou quais ambientes o bug é reproduzível._

1. _**OBS: Essa informação precisa estar disponível na issue e se for o caso, basta copiar e colar, colocar um link e explicitar em quais ambientes é possível reproduzir.**_

2. _**OBS: Bugs não reproduzíveis podem ser encaminhados diretamente a issue, porém no evento do time optar pela não correção, a issue deverá estar devidamente documentada e linkada nesta sessão para ser acessível no futuro.**_

>Ex_1: 
>- Bug não reproduzível, mais informações na issue.[#98](https://gitlab.com) 

>Ex_2:
>- 1. Entre em qualquer produto tal qual [Coca-cola](https://gitlab.com).
>- 2. Adicione o produto ao carrinho.
>- 3. Clique no carrinho na parte superior direita da aplicação.
>- 4. Aperte no botão com símbolo de (+) ao lado do produto.
>- 5. Veja que o botão não dá nenhum feedback apesar da pequena demora para a quantidade de itens serem alterados no campo que mostra a quantidade logo ao lado do botão.

## Proposed Solution:

_Solução proposta para o dado problema._

1. _**OBS: Se não for algo de domínio de todo o time ou pelo menos dos reviewers, é importante especificar o porque aquela abordagem está sendo tomada.**_

>Ex_1: 
>- O melhor caso é adicionar uma propriedade de loading no componente do botão. Assim sendo possível minar a possibilidade de multiplas requests por multiplos cliques e também retornar um feedback de que algo está acontecendo para o usuário.

## Acceptance Requirements:
_Os mesmos requisitos de aceitação, o que o seu Merge está corrigindo e quais passos ele deve obedecer._

>Ex:
> - [x] Deixar botão em estado suspenso após o click.
> - [x] Checar retorno da api sobre valor e quantidade.
> - [x] Retornar uma mensagem de erro caso receba um retorno inesperado da Api.
> - [x] Retornar botão para estado inicial e mostrar quantidade correta no contador ao receber o OK da Api.

## Additional/External Resources:
_Links para documentação de assets ou qualquer recurso adicional se foram utilizados._

- _Estão inclusos em recursos adicionais qualquer parte advinda de terceiros, normalmente Libs que não são padrões do projeto._ 
- _No caso da Vtex, apps extras utilizados deverão ser colocados com seus respectivos links de documentação e ou base de código aqui nesta sessão._

1. _**OBS: Algumas features necessitam da utilização da Master Data e ou estão linkadas de alguma forma a esquemas/informações que existem fora do contexto da aplicação, nesse caso, é importante que essas informações sejam documentadas nesta parte ou em um README.md.**_
   1. - Esse comportamento é necessário para facilitar a manutenção de código e documentação se caso a pessoa que possue o domínio da aplicação venha a se ausentar.
   2. - Colocar o esquema ou algum outro tipo de informação que explicite como o esquema funciona fica a critério de quem está criando a MR ou lógica interna do time. O importante é que exista algum tipo de documentação a respeito. 

2. _**OBS: Considerando que boa parte dos Apps da Vtex não possuem uma boa documentação, pode-se linkar qualquer arquivo o qual tenha servido de base e ou possua as funções/funcionalidades que tenham sido utilizadas.**_


>Ex:
>- [Vtex-instore-profile](https://github.com/vtex-apps/instore-profile)
```json
--> Esquema da master data utilizado para guardar dados dos pagamentos para calculos da loja.

Master-Data-Info:
- data-entity: Instore
- schema: instore-customers
- endpoint_to_check_info: Search Documents
- schema_body: {
    "customers_amount": 6,
    "table_number": 13,
    "payment_type": "Visa",
    "timestamp": "2020-08-17T03:29:31+00:00",
    "value": 123.12,
    "CPF_CNPJ":"012.321.123-42"
}
```

## Related Changes:

_Alguma mudança específica que não estava prevista para ser feita, porém, foi necessária pois estava relacionada ao escopo do seu MR_

_Se caso for um tipo de bugfix que precise de mudança de documentação, adicionar também link para documentação e ou onde é possível encontra-la._

>Ex:
>- Correção de bug que não permitia armazenamento de informação no local storage através de função no contexto.

## Demo/Workspace:

_Devido a natureza do bug, há a necessidade de demonstrar como o comportamento estava e como está, seja através de um link para a issue que já possui essa informação em forma de gif/vídeo/image ou seja através dos steps realizados pelo próprio desenvolvedor._

- _Obviamente também é necessário linkar o workspace ou alguma outra forma de fácil observação sobre o comportamento que está sendo corrigo pelo Merge Request._

>Ex: 
>- [Vídeo/Gif/Foto demonstrando comportamento atual (errado)](https://gitlab.com/)
>- [Vídeo/Gif/Foto hospedado em outro lugar demonstrando comportamento esperado](https://gitlab.com/) ou [Workspace corrigido](https://gitlab.com/)

## Test Environment:
_Descrever aqui, se existir, como reproduzir testes unitários/integração e em quais ambientes tais testes ocorreram ou são possíveis de ser executados._

- _Se possível e ou aplicável, um overview do coverage, seja em forma de foto/gif/vídeo, fica a critério de quem está criando o MR ou lógica interna do time._


>Ex: 
>- ```npm run tests``` executa os testes unitários.
>- Testes executados no chrome e no firefox.
>- Não foram executados no IE pois não é necessário o suporte.