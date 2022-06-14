## Introdução

Seu desafio agora será implementar uma feature nesta aplicação: a autenticação 
do Firebase.

Nas próximas aulas, eu mostrarei como autenticar através da conta do google. 
Assim, não é necessário se preocupar com força de senha do usuário. Recomendo 
que você faça o mesmo.

---

## O que você precisa fazer

---

### Quando o usuário está deslogado

Quando o usuário estiver deslogado, apenas o link de login deve ser exibido 
no navbar, desta forma:

![image](https://user-images.githubusercontent.com/29297788/154863093-fc2ae7c8-fe7f-4436-815d-502851f646f3.png)

Note também que há uma mensagem no centro da tela, "Faça login para ver as 
frases". Use o CSS do Materialize para estilizar a mensagem.

Quando o link `login` for clicado, o modal abaixo deve ser exibido.

![image](https://user-images.githubusercontent.com/29297788/154863206-793c8dc8-90f9-496f-bed5-e1092f8ad4ae.png)

Ao clicar no botão `Entrar com Google`, o popup padrão do google deverá ser 
aberto para o usuário entrar com a conta do Google dele.

![google-popup](https://user-images.githubusercontent.com/29297788/154863492-4c33d340-eb91-4414-b979-75b00db06db6.jpg)

---

### Quando o usuário fizer login

Ao entrar, o modal deve ser fechado, o navbar deverá exibir os links `Adicionar frase`, `Conta` e `Logout` e logo abaixo, a lista de frases deverá ser exibida.

![image](https://user-images.githubusercontent.com/29297788/154863806-30cfecbb-d1a0-41bd-b001-5ee6d7d12879.png)

No exemplo acima, o usuário possui duas frases salvas. Uma do filme "O Mágico de Oz" e outra do filme "E.T.: O Extraterreste". Quando não houverem frases salvas, a listagem de frases não deve ser exibida.

A listagem de frases é um componente do Materialize, semelhante à um accordion. Quando o título do filme é clicado, o item se abre e a frase é exibida.

![image](https://user-images.githubusercontent.com/29297788/154863914-9b929a85-98a4-4344-b737-c77117345eef.png)

Quando o link `Adicionar frase` for clicado, o modal abaixo deve ser aberto.

![image](https://user-images.githubusercontent.com/29297788/154864271-371dd299-a770-4a1f-9a21-e195a1688868.png)

Quando o form do modal acima for enviado, o modal deve ser fechado e o novo filme adicionado deve estar na lista, sem que seja necessário recarregar a página.

![image](https://user-images.githubusercontent.com/29297788/154864312-bbbb1cee-233f-4f3e-95fd-5348aa9a7067.png)

Quando o link `Conta` for clicado, o modal abaixo deve ser aberto.

![image](https://user-images.githubusercontent.com/29297788/154864384-924fdc8d-de79-41d1-a2b8-4c9267d528da.png)

Este modal deve conter o nome e o email do usuário logado na aplicação. 

Ao clicar em qualquer parte fora do modal acima, ele deve ser fechado.

---

### Quando o usuário fizer logout

Quando o link `Logout` for clicado, apenas o link `Login` deve ser exibido 
no navbar e "Faça login para ver as frases" deve ser exibida no centro da tela.

![image](https://user-images.githubusercontent.com/29297788/154864442-b4bd78c1-8667-4fe3-a769-8c7586c1672e.png)

---

## Links

Vou deixar abaixo os links das documentações nas quais você precisará 
pesquisar para fazer este desafio:

- [Firebase](https://firebase.google.com/docs)
- [Materialize](https://materializecss.com/)
- [MDN Web Docs](https://developer.mozilla.org/en-US/)

---

## JavaScript do Materialize

Eu não indicaria isso se você não estivesse nessa etapa, mas se sentir que 
sabe o que está fazendo, você pode usar funcionalidades JavaScript do 
Materialize.

Você já sabe como implementar modal (popup) e accordion com JS puro, já sabe 
como isso funciona por baixo dos panos.

Usar modal e accordion do Materialize pode te fazer ganhar tempo, afinal 
o foco aqui é que você aprenda a implementar a autenticação com o Firebase. 

---

## Dicas

Leia as dicas abaixo apenas se travar em algum ponto e precisar de ajuda.

---

### Localhost

Se ao clicar em "Entrar com Google" for exibida uma mensagem dizendo que 
o seu domínio não está autorizado para operações de autenticação, dê uma 
olhada em `Authorized domains`, na aba `Sign-in method` da tela 
`Authentication` no console do Firebase, e também na aula 
`Configurando o ambiente - Aula 01-03` da etapa 01.

---

### Links invisíveis

Por padrão, todos os links estão com uma classe CSS `hide`, do Materialize.

---

### Modais

Como os modais utilizados são os do Materialize, a exibição e fechamento deles 
deve ser manipulada seguindo a documentação JavaScript dessa biblioteca.

---

### app.js

O `app.js` já contém os `import` com a versão do Firebase que deve ser usada, 
por que essa será a versão mostrada nas próximas aulas.

Se quiser, você pode usar uma versão diferente depois.
