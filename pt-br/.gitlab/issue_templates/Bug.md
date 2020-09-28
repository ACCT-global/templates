<!-- NEM TODOS OS CAMPOS EXISTIRÃO EM TODA FEATURE, POR FAVOR DELETAR OS CAMPOS DESNECESSÁRIOS. -->

## Overview:

<!--
É importante uma descrição que faça sentido e esteja bem documentada, para que seja possível uma reação mais rápida e mais acertiva do time.
-->

- Ao entrar em `mystore.com`, adicionar qualquer produto no carrinho e tentar completar uma compra, ao chegar no passo de adicionar E-mail do cliente na entrada do checkout, a aplicação me permite pular este passo, assim ignorando a obrigatoriedade do de E-mail.

## Steps to reproduce:
<!--
Uma descrição dos passos necessários para reprodução do bug.

Utilize uma lista numerada para explicitar a ordem dos passos a serem seguidos

Caso não tenha sido possível de reproduzir, é necessário explicitar tudo que tenha sido tentado.
-->

- **Erro encontrado apenas no navegador Internet Explorer 9.**

1. Abra o navegador Internet Explorer 9.
2. Vá até `mystore.com/seller`.
2. Adicione qualquer item ao carrinho.
3. Vá no seu carrinho e clique em finalizar compra.
4. Na parte de adicionar seu E-mail, clique no botão `Avançar`.
5. Veja que o E-mail não está sendo obrigatório como é o esperado.

## The current *Bug* behavior:

<!-- Qual o comportamento atual do BUG. -->

- Atualmente, após tentar finalizar qualquer compra dentro de `mystore.com` utilizando o navegador Internet Explorer 9, o E-mail não encontra-se obrigatório.

## The expected *correct* behavior:

<!-- Qual o comportamento esperado. -->

- O comportamento esperado é que não seja possível avançar para além deste passo sem a adição do E-mail de usuário em todos os navegadores os quais o suporte é necessário.

## Relevant logs and/or screenshots:

<!--
Adicionar aqui qualquer `log` relavante, utilizando-se de blocos de código (```) para formatar saídas de console, códigos e etc.

Se houver, adicionar também gif, foto ou vídeo do comportamento considerado BUG.
-->

## Possible fixes:

<!-- 
Possibilidades de contorno ou resolução do BUG que já foram aplicadas, caso existam. 

Tdicionar link para `FAQ` ou outros pontos de informações que levem a um melhor entendimento deste comportamento, caso existam.
-->