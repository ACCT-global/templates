# Improvement

## Why:
_Uma explicação do porque o código necessita de tais melhorias, caso exista uma issue que explicite algum dos problemas o qual esse MR resolve, linke-a também._

> Ex:
>- Componente ```timer.tsx``` possui uma complexidade muito alta com o uso de inúmeros estados internos os quais podem ser recebidos por propriedades assim facilitando testes e a utilização desse componente.
>- Utils ```getUserPaymentInformation``` possui muitas ramificações referentes as várias opções de pagamento. Uma maior abstração desse conceito se torna necessária para que a função seja melhor reutilizada e tais validações se tornem mais gerais.
>- useEffect o qual faz o fetch de informações no componente ```UserCard``` está dando trigger a cada mudança de informação do usuário, seja ela repetida ou não. Esta informação pode ser recebida através de propriedade e o componente pode receber a propriedade de memoization para que seja re-renderizado somente quando as propriedades reebidas forem diferentes das propriedades recebidas anteriormente.
>- Coverage de testes está baixa devido a dificuldade de testar alguns componentes muito intrincados como o próprio ```UserCard```, após a mudança para receber propriedades em vez de um estado interno, será possível aumentar sua coverage para 100%. 
> - ### **Related Issues:**
>   - [#12](https://google.com.br)
>   - [#25](https://google.com.br)
>   - [#99](https://google.com.br)

## Overview:
_Explicitar suas mudanças de forma simples._

> Ex:
>- Melhor legibilidade no ```component/timer.tsx```.
>- Removendo complexidade ciclomática.
>- Retirando lógica de useEffect desnecessária e utilizando props.
>- Aumentando Coverage dos testes.

## Test Environment:
_Se for possível a aplicação de testes unitários/integração, descrever aqui como reproduzi-los e em quais ambientes tais testes ocorreram._

_Se possível e ou aplicável, um overview do coverage, seja em forma de foto/gif/vídeo, fica a critério de quem está criando o MR._

_Sempre utilizar da comparação de coverage ou forma similar de garantir o funcionamento da aplicação como um todo. Nada deve quebrar._

>Ex: 
>- ```npm run tests``` executado
>- [Foto de coverage anterior as mudanças]()
>- [Foto de coverage após mudanças]()
