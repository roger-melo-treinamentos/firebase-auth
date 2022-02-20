## Introdução

Seu desafio agora será usar o sistema de autenticação do Firebase nesta 
aplicação.

Nas próximas aulas, eu mostrarei como autenticar através da conta do google. 
Assim, não é necessário se preocupar com força de senha do usuário.

---

## O que você precisa fazer

Esta aplicação irá exibir frases de filmes apenas para quem estiver logado. 

Quando o usuário estiver deslogado, apenas o link de login deve ser exibido 
no navbar, desta forma:

![image](https://user-images.githubusercontent.com/29297788/154863093-fc2ae7c8-fe7f-4436-815d-502851f646f3.png)

Note também que há uma mensagem no centro da tela, "Faça login para ver as 
frases". Use o CSS do Materialize para estilizar a mensagem.

Ao clicar em `login`, o modal abaixo deve ser exibido.

![image](https://user-images.githubusercontent.com/29297788/154863206-793c8dc8-90f9-496f-bed5-e1092f8ad4ae.png)

Ao clicar no botão `Entrar com Google`, um popup deverá ser aberto para o 
usuário entrar com a conta do Google dele.

![google-popup](https://user-images.githubusercontent.com/29297788/154863492-4c33d340-eb91-4414-b979-75b00db06db6.jpg)

Ao entrar, o navbar deverá exibir os links `Adicionar frase`, `Conta` e `Logout` e logo abaixo, a lista de frases deverá ser exibida.

![image](https://user-images.githubusercontent.com/29297788/154863806-30cfecbb-d1a0-41bd-b001-5ee6d7d12879.png)

No exemplo acima, o usuário possui duas frases salvas. Uma do filme "O Mágico de Oz" e outra do filme "E.T.: O Extraterreste". Quando não houverem frases salvas, a listagem de frases não deve ser exibida.

A listagem de frases é um componente do Materialize, semelhante à um accordion. Quando o título do filme é clicado, o item se abre e a frase é exibida.

![image](https://user-images.githubusercontent.com/29297788/154863914-9b929a85-98a4-4344-b737-c77117345eef.png)


---

## Links

Vou deixar abaixo os links das documentações que você precisará consultar 
para fazer este desafio:

- [Firebase](https://firebase.google.com/docs)
- [Materialize](https://materializecss.com/)
- [MDN Web Docs](https://developer.mozilla.org/en-US/)

---

## JavaScript do Materialize

Eu não indicaria isso se você não estivesse nessa etapa, mas se sentir que 
sabe o que está fazendo, você pode usar funcionalidades JavaScript do 
Materialize.

Você já sabe como implementar modal (popup) e accordion com JS puro.

Usar modal e accordion do Materialize pode te fazer ganhar tempo, afinal 
o foco aqui é que você aprenda a implementar a autenticação com o Firebase. 

---

## Dicas

Leia as dicas abaixo apenas se travar em algum ponto e precisar de ajuda.

### Localhost
The current domain is not authorized for OAuth operations
### Links invisíveis
### Modais e Accordion