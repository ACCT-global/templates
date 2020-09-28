# Hotfix

## Overview:
_Uma explicação do porque este hotfix é necessário._

- _Caso este erro o qual está sendo corrigido em forma de hotfix tenha origem em algum MR de fácil acesso, o link do MR anterior se torna obrigatório, caso não haja uma issue, crie e faça o respectivo link._

>Ex: 
> - Api não está retornando erro de Input quando o body da requisição de criar um novo usuário vem vazio.

> - ### **Related Issues:**
>   - [#10](https://google.com.br)

## Proposed Solution:

_Solução proposta para o dado problema._

1. _**OBS: Se não for algo de domínio de todo o time ou pelo menos dos reviewers, é importante especificar o porque aquela abordagem está sendo tomada.**_

>Ex_1: 
>- O melhor caso é adicionar uma propriedade de loading no componente do botão. Assim sendo possível minar a possibilidade de multiplas requests por multiplos cliques e também retornar um feedback de que algo está acontecendo para o usuário.

## Acceptance Requirements:
_O que o seu Merge está corrigindo e quais passos ele deve obedecer para chegar ao comportamento esperado._

>Ex:
> - [x] Validar se Body da requisição está vindo vazio do front-end.
> - [x] Retornar status 200 com a informação do novo usuário para o front-end.
> - [x] Retornar status 400 (Erro de input) com mensagem a respeito de body obrigatório em caso de receber body vazio.
> - [x] Retornar status 500 com "internal error" caso ocorra algum erro de processamento interno da API.

## Demo/Workspace:

_Devido a necessidade da rápida correção, é provável que o workspace ou a forma de teste seja diferente, sendo assim, sempre que possível, seguir a lógica de linkar um workspace diferente ou alguma outra forma de fácil observação sobre o comportamento que está sendo corrigo pelo Merge Request._

>Ex: 
>- [Vídeo/Gif/Foto demonstrando comportamento atual (errado)](https://gitlab.com/)
>- [Vídeo/Gif/Foto hospedado em outro lugar demonstrando comportamento esperado](https://gitlab.com/) ou [Workspace novo com correção](https://gitlab.com/)

## Test Environment:
_Descrever aqui, se existir, como reproduzir testes unitários/integração e em quais ambientes tais testes ocorreram ou são possíveis de ser executados._

- _Se possível e ou aplicável, um overview do coverage, seja em forma de foto/gif/vídeo, fica a critério de quem está criando o MR ou lógica interna do time._


>Ex: 
>- ```npm run tests``` executa os testes unitários.
>- Testes executados no chrome e no firefox.
>- Não foram executados no IE pois não é necessário o suporte.