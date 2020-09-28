<!-- NÃO DEIXE NADA DO BOILERPLATE QUE NÃO SEJA ÚTIL A DESCRIÇÃO DO SEU MR -->

## Overview:
<!-- Uma explicação do porque este hotfix é necessário.
Caso este erro o qual está sendo corrigido em forma de hotfix tenha origem em algum MR de fácil acesso, o link do MR anterior se torna necessário para facilitar a inserção do contexto da correção. -->

- Api não está retornando erro de Input quando o body da requisição de criar um novo usuário vem vazio. [MR #12]()

- ### **Related Issues:**
  - [#10](https://google.com.br)

## Proposed Solution:

<!--
Solução proposta para o dado problema e por qual motivo essa solução foi escolhida. 
-->

- O melhor caso é adicionar uma propriedade de loading no componente do botão. Assim sendo possível minar a possibilidade de multiplas requests por multiplos cliques e também retornar um feedback de que algo está acontecendo para o usuário.


## Acceptance Requirements:
<!-- Requisitos de aceitação do seu Hotfix. -->

- [x] Validar se Body da requisição está vindo vazio do front-end.
- [x] Retornar status 200 com a informação do novo usuário para o front-end.
- [x] Retornar status 400 (Erro de input) com mensagem a respeito de body obrigatório em caso de receber body vazio.
- [x] Retornar status 500 com "internal error" caso ocorra algum erro de processamento interno da API.

## Demo/Workspace:
<!-- Workspace ou forma simples de demonstração. -->

- [Vídeo/Gif/Foto demonstrando comportamento atual (errado)](https://gitlab.com/)
- [Vídeo/Gif/Foto hospedado em outro lugar demonstrando comportamento esperado](https://gitlab.com/) ou [Workspace novo com correção](https://gitlab.com/)

- [Workspace]()

## Test Environment:
<!-- Como reproduzir testes unitários/integração e em quais ambientes tais testes ocorreram ou são possíveis de ser executados, se aplicável, um overview do coverage. -->

- ```npm run tests``` executa os testes unitários.
- Testes executados no chrome e no firefox.
- Não foram executados no IE pois não é necessário o suporte.