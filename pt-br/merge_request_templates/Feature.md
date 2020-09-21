# Feature

## Task Definition
_Aqui vai uma explicação do que o seu MR se dispôe a fazer, sempre junto do link da issue relacionada facilitando assim a navegação entre o Merge Request e a task no gitlab. (Não é legal sair procurando no board cada task de cada MR.)_

> Ex: 
>- Adicionando lógica de instore no checkout.
> - ### **Related Issues:**
>   - [#13](https://google.com.br)

## Additional/External Resources
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

## Acceptance Requirements
_Aqui vem uma explicação geral de quais passos a sua feature necessita para ser aceita (estar completa)._

- _Podendo ser uma cópia dos passos que já estão na task a princípio, porém sempre lembrando que essa parte da descrição será aquela levada com maior rigor para o review pois todos os passos são necessários para a aceitação dessa feature._

- _Também serve como um lembrete para quem está abrindo o MR, de quais comportamentos são primordiais para que a feature exerça a função desejada._

>Ex:
> - [x] Não impactar no funcionamento de outras funcionalidades.
> - [x] Aceitar outras formas de pagamento além de cartão de crédito.
> - [x] Aceitar pagamento em espécie.
> - [x] Opção de receber o pedido em uma mesa.
> - [x] Opção de aviso remoto através de E-mail/Sms sobre pedido pronto.

## Not Related changed 

_Alguma mudança específica que não estava prevista para ser feita, porém, foi necessária pois estava relacionada ao escopo do seu MR_

>Ex:
>- Correção de bug que não permitia armazenamento de informação no local storage através de função no contexto.

## Demo/Workspace

_Sempre será necessário a utilização de um workspace próprio para o desenvolvimento da feature e ou uma demonstração em forma de vídeo/gif/foto para facilitar o review._

>Ex: [Vídeo/Gif/Foto demonstrando feature em funcionamento no checkout](https://gitlab.com/) ou [Workspace](https://gitlab.com/)


## Test Environment
_Descrever aqui, se existir, como reproduzir testes unitários/integração e em quais ambientes tais testes ocorreram ou são possíveis de ser executados._

- _Se possível e ou aplicável, um overview do coverage, seja em forma de foto/gif/vídeo, fica a critério de quem está criando o MR ou lógica interna do time._


>Ex: 
>- ```npm run tests``` executa os testes unitários.
>- Testes executados no chrome e no firefox.
>- Não foram executados no IE pois não é necessário o suporte.