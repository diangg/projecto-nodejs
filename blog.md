Como criar um projecto node

[banner]

--Introducao:
    Bom dia, Boa tarde, Boa noite colegas. Hoje iremos criar o nosso primeiro projecto node js de uma forma muito facil e rapida.
    Bora mergulhar?!
    [gif]


    "Node.js" e uma biblioteca da linguagem Javascript que permite criar aplicacoes web. Ele é caracterizado por ser uma linguagem muito fácil e rápida, feita do famosinho Javascript

--Desenvolvimento

    Todo projecto em node js é constituído por 5 pastas importantes são elas:

        -public [icon] - Controller [icon]
        -views [icon]   -Models[icon]
        -routes [icon]

    Mas o que é essa sopa de letrinhas? Calma, vamos entender elas tranquilamente

    -public: Esta é a pasta onde ficam as nossas imagems, os arquivos de css e javascript😉

    -views: Está é pasta onde ficam os nossos arquivos html, os famosos formulários, layouts ou páginas 📝

    -Models: Aqui fica os arquivos de base de dados (Veremos no próximo post)🎲

    - Routes: Aqui ficam as rotas ou caminhos que levam a páginas do nosso alicativo ex: "/videos", "/professores/delfin

    -Controllers: Aqui ficam os arquivos do programação, o código que vamos implementar nesta rota. Ex: código de cadastrar Usuário numa rota "/usuarios/cadastro"

    Para visualizar os ícones das pastas, podemos baixar a extensão _material icon theme_ no VS CODE. Para baixar extensões no Visual Studio Code é necessário internet ou saldo de dados (africell de 200kz)

    [foto das extensoes]

    E assim fica o nosso projecto

    
    [foto do estrutura do projecto]

    Falta apenas um passo, criar o arquivo principal do projecto: o app.js. Basicamente criamos um arquivo chamado app.js, onde existirá o nosso projecto

    [foto da estrutura com o app.js]

    ---> Mexendo no app.js

    Depois de criadas as pastas, vamos entender uma coisa:

    O Node js e uma biblioteca do Javascript, sendo uma biblioteca, ela contém vários livros que podemos utilizar, podemos requerir estes livros da biblioteca node e usá-los 

    Vamos usar um livro chamado Express, que nos permite colocar a nossa aplicação web nos navegadores dos nossos computadores

    Para instalar o Express, usamos o comando:

        npm install express --save
    Para requerir e usar o Express no nosso arquivo app.js, usamos a função require()

        const express = require("express")
        
    a constante express, depois de receber o require("express") torna- se uma função que usaremos na variável app

        const app = express()

    No fim do arquivo app.js, utilizamos o método listen(), do express, onde passamos a porta e a mensagem de início do aplicativo

        app.listen(8081,function(){
            console.log("Servidor rodando em http://localhost:8081")
        })



        





