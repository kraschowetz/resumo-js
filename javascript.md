# javascript no projeto

o javascript (.js) usado no projeto valida o logiun do usuário.

em pseudo-código o js ficaria algo assim:

~~~
if nome == "aluno1909" && senha == "Setembro@2024" {
	efetuar_login();
}
else {
	exibir_erro();
}
~~~
-------------------------------------------------------

# como funciona o Javascript?

## declarando funcões:

~~~
function nome() {
    //fazer algo
}
~~~

## declarando váriaveis:

~~~
let numero = 0;
~~~

- o javascript não tem tipos de váriaveis
- em alguns casos se usa var para declarar varáveis, mas é recomendado usar o let

## explicando o código:

~~~
function validarLogin() { ...
~~~
declarando a funcão de validar login, ela vai ser chamada pelo html

~~~
let nomeUsuario = document.getElementById('txtUsuario').value;
let senha = document.getElementById('txtSenha').value;
~~~
declarando a váriavel nomeUsuario e senha.
o 'document.getElementById()' pega um objeto no html baseado no ID, depois o '.value' pega o valor que foi digitado na caixa de usuário e senha.
o valor dessas caixas é colocado nas variáveis.

~~~
alert("lorem ipsum");
~~~
é parecido com System.out.println();

~~~
window.location.href = './teste.html';
~~~
muda a página para 'teste.html'

## js no html

~~~
<script src="validacao.js">
~~~
- importa o javascript no documento html
- geralmente colocado no final do <body>

~~~
<button onclick="validarLogin;return false;">
~~~
declarando um <botão>, o onclick diz qual funcão do javascript ele vai executar, o return false; é uma convencão de boa prática, não é nescessário mas é bão ter
