<!-- NÃO DEIXE NADA DO BOILERPLATE QUE NÃO SEJA ÚTIL A DESCRIÇÃO DO SEU MR -->

## Fix Type:
<!-- Deletar checkboxes que não são se aplicam ao Merge Request. -->

- [x] - Minor Bugfix.

- [ ] - Bugfix with Breaking Change.

- [ ] - Change requires a Documentation update.

## Overview:
<!-- Descrição do Bug. -->

> - Comportamento atual: Botão de adicionar mais 1 item ao carrinho de compras não dá nenhum feedback que a ação ocorreu ao ser clicado.
> - Comportamento esperado: Botão deve entrar em um estado suspenso tanto para dar um feedback para o usuário quanto para impedir adições subsequentes antes que a mudança de quantidade ocorra.


- ### **Related Issues:**
  - [#12](https://google.com.br)
  - [#25](https://google.com.br)
  - [#99](https://google.com.br)

## Reproduction Steps:
<!-- 
- Essa informação precisa estar disponível na issue e se for o caso, basta copiar e colar, colocar um link e explicitar em quais ambientes é possível reproduzir.

- Bugs não reproduzíveis podem ser encaminhados diretamente a issue, porém caso o time chegue a optar pela não correção, a issue deverá estar devidamente documentada e linkada nesta sessão para ser acessível no futuro. 
-->

>Ex_1: 
>- Bug não reproduzível, mais informações na issue.[#98](https://gitlab.com) 

>Ex_2:
>- 1. Entre em qualquer produto tal qual [Coca-cola](https://gitlab.com).
>- 2. Adicione o produto ao carrinho.
>- 3. Clique no carrinho na parte superior direita da aplicação.
>- 4. Aperte no botão com símbolo de (+) ao lado do produto.
>- 5. Veja que o botão não dá nenhum feedback apesar da pequena demora para a quantidade de itens serem alterados no campo que mostra a quantidade logo ao lado do botão.

## Proposed Solution:

<!--
Solução proposta para o dado problema e por qual motivo essa solução foi escolhida. 
-->

>Ex_1: 
>- O melhor caso é adicionar uma propriedade de loading no componente do botão. Assim sendo possível minar a possibilidade de multiplas requests por multiplos cliques e também retornar um feedback de que algo está acontecendo para o usuário.

## Acceptance Requirements:
>Ex_1:
> - [x] Deixar botão em estado suspenso após o click.
> - [x] Checar retorno da api sobre valor e quantidade.
> - [x] Retornar uma mensagem de erro caso receba um retorno inesperado da Api.
> - [x] Retornar botão para estado inicial e mostrar quantidade correta no contador ao receber o OK da Api.

## Additional/External Resources:
<!-- Qualquer tipo de recurso externo que tenha sido utilizado, adicionar documentação também. -->


## Related Changes:

<!-- Alguma mudança específica que não estava prevista para ser feita, porém, foi necessária -->

<!-- Caso exista uma necessidade de mudança de documentação, adicionar aqui o link/caminho para nova documentação atualizada ou onde é possível encontra-la. -->

>Ex_1:
>- Correção de bug que não permitia armazenamento de informação no local storage através de função no contexto.

## Demo/Workspace:
>Ex_1: 
> - [Vídeo/Gif/Foto demonstrando comportamento atual (errado)](https://gitlab.com/)
> - [Vídeo/Gif/Foto hospedado em outro lugar demonstrando comportamento esperado](https://gitlab.com/) ou [Workspace corrigido](https://gitlab.com/)

## Test Environment:
<!-- Como reproduzir testes unitários/integração e em quais ambientes tais testes ocorreram ou são possíveis de ser executados, se aplicável, um overview do coverage. -->

>Ex_1:
>- ```npm run tests``` executa os testes unitários.
>- Testes executados no chrome e no firefox.
>- Não foram executados no IE pois não é necessário o suporte.