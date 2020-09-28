<!-- NÃO DEIXE NADA DO BOILERPLATE QUE NÃO SEJA ÚTIL A DESCRIÇÃO DO SEU MR -->

## Overview:
<!-- Descrição simples do que sua feature precisa fazer. -->

- Adicionando lógica de instore no checkout. [#123](https://gitlab.com/)

## Additional/External Resources:
<!-- Links para documentação de assets ou qualquer recurso adicional se forem adicionados.

**OBS_1: Algumas features necessitam da utilização da Master Data e ou estão linkadas de alguma forma a esquemas/informações que existem fora do contexto da aplicação, nesse caso, é importante que essas informações sejam documentadas nesta parte ou em um README.md.**
 - Esse comportamento é necessário para facilitar a manutenção de código e documentação se caso a pessoa que possue o domínio da aplicação venha a se ausentar.
 - Colocar o esquema ou algum outro tipo de informação que explicite como o esquema funciona fica a critério de quem está criando a MR. O importante é que exista algum tipo de documentação a respeito.  -->

## Acceptance Requirements:
<!-- Passo a passo e quais requerimentos a sua MR precisa executar para ser aceita -->

- [x] Aceitar outras formas de pagamento além de cartão de crédito.
- [x] Aceitar pagamento em espécie.
- [x] Opção de receber o pedido em uma mesa.
- [x] Opção de aviso remoto através de E-mail/Sms sobre pedido pronto.

## Related Changes:

<!-- Alguma mudança específica que não estava prevista para ser feita, porém, foi necessária -->

- Correção de bug que não permitia armazenamento de informação no local storage através de função no contexto.

## Demo/Workspace:
<!-- Workspace ou forma simples de demonstração. -->

- [Vídeo/Gif/Foto demonstrando feature em funcionamento no checkout](https://gitlab.com/)

## Test Environment:
<!-- Como reproduzir testes unitários/integração e em quais ambientes tais testes ocorreram ou são possíveis de ser executados, se aplicável, um overview do coverage. -->

- ```npm run tests``` executa os testes unitários.
- Testes executados no chrome e no firefox.
- Não foram executados no IE pois não é necessário o suporte.