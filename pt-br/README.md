# Boilerplates para utilização em Merge Requests.

## Pros:
  1. Informações centralizadas. Seja recursos utilizados, link para task, requisitos de aceitação e etc..
   
  2. Apesar da lógica de Changelog, é necessária uma forma que possibilite maior controle por parte de quem utiliza o código diariamente, para que mudanças complexas possam ser reversíveis e melhor gerenciadas.
   
  3. Projetos nos quais existem multiplos ambientes e que há a possibilidade da adição de mais ambientes, possuem uma maior necessidade de controle sobre quais mudanças se encontram ou irão entrar em cada ambiente.
   
  4. Facilitar o review, considerando que, de antemão, já será possível ter uma noção do que se espera do MR( qual problema/necessidade este MR se dispõe a resolver, quais recursos externos estão sendo utilizados, etc).

## Cons:
  1. Mais tempo por parte de quem está abrindo o MR para preencher a descrição da forma necessária.

  2. Alguns Merge Requests podem, por algum motivo, não se encaixar perfeitamente nos boilerplate já existentes.

  3. Necessidade de atenção por parte de quem está abrindo a MR para que mudanças feitas de última hora também sejam adicionadas ao contexto da descrição para não atrapalhar o review e o fluxo estipulado pela própria lógica da descrição.

# Informações adicionais.
- Dentro da pasta `merge_request_templates` existem explicações detalhadas do que deve ser preenchido com exemplos básicos pata cada tópico considerando o momento em que tais templates estejam sendo preenchidos.
- No momento, os templates são divididos entre;
  - `Bug`
  - `Feature`
  - `Hotfix`
  - `Improvement`
