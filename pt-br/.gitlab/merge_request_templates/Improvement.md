<!-- NÃO DEIXE NADA DO BOILERPLATE QUE NÃO SEJA ÚTIL A DESCRIÇÃO DO SEU MR -->

## Why?
<!-- Uma explicação do porque o código necessita de tais melhorias. -->

> Ex:
>- Componente ```timer.tsx``` possui uma complexidade muito alta com o uso de inúmeros estados internos os quais podem ser recebidos por propriedades assim facilitando testes e a utilização desse componente.
>- Utils ```getUserPaymentInformation``` possui muitas ramificações referentes as várias opções de pagamento. Uma maior abstração desse conceito se torna necessária para que a função seja melhor reutilizada e tais validações se tornem mais gerais.
>- useEffect o qual faz o fetch de informações no componente ```UserCard``` está dando trigger a cada mudança de informação do usuário, seja ela repetida ou não. Esta informação pode ser recebida através de propriedade e o componente pode receber a propriedade de memoization para que seja re-renderizado somente quando as propriedades reebidas forem diferentes das propriedades recebidas anteriormente.
>- Coverage de testes está baixa devido a dificuldade de testar alguns componentes muito intrincados como o próprio ```UserCard```, após a mudança para receber propriedades em vez de um estado interno, será possível aumentar sua coverage para 100%. 

## Overview
<!-- Explicitar suas mudanças de forma simples. -->

> Ex:
>- Melhor legibilidade no ```component/timer.tsx```.
>- Removendo complexidade ciclomática.
>- Retirando lógica de useEffect desnecessária e utilizando props.
>- Aumentando Coverage dos testes.

## Test Environment
<!-- Se possível e ou aplicável, um overview do coverage, seja em forma de foto/gif/vídeo, fica a critério de quem está criando o MR. -->

>Ex: 
>- ```npm run tests``` executado
>- [Foto de coverage anterior as mudanças]()
>- [Foto de coverage após mudanças]()
