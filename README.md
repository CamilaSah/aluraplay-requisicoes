![JavaScript-requisicoes](https://github.com/CamilaSah/aluraplay-requisicoes/assets/128820692/df9c3e39-ab58-44f7-a6f2-6d786eea2bf0)
![Static Badge](https://img.shields.io/badge/Status-Conclu%C3%ADdo-%2391DCFF)

<h1>AluraPlay</h1>
O AluraPlay é uma plataforma de compartilhamento de vídeos da Alura. O projeto inicial tinha somente quatro vídeos, um header com o logo no canto superior esquerdo da tela, uma barra de pesquisa no canto superior ao centro e um botão de inserção de novos vídeos no campo superior direito. O projeto já tinha CSS e HTML prontos.
<br>
O resultado proposto no curso era de chegar em uma página com uma listagem de vários vídeos, inseridos através de uma API, no qual era possível clicar no botão superior direito e inserir um novo vídeo.

Para realizar esse projeto, aprendeu-se os seguintes temas:
* Como instalar o NodeJS e o json-server no projeto;
* Como Mockar uma API com o auxílio do json-server;
* Como criar requisições GET e POST para essa API;
* Revisão dos conceitos de JavaScript assíncrono;
* Criação da funcionalidade de pesquisa;
* Manipulação do DOM;
* Tratamento dos erros de requisições.

## Screenshots
![Screenshot da tela inicial do AluraPlay](https://imgur.com/aymxEsh.png)
![Screenshot da tela do formulário do AluraPlay](https://imgur.com/ShNADf2.png)

## :hammer: Funcionalidades do projeto
- `Fazer busca de vídeos`: quando o usuário escrever a palavra chave a ser pesquisada e clicar no botão de buscar, somente os vídeos com aquele termo de busca aparecerão na tela.
- `Inserir novos vídeos e aparecer na tela inicial`: quando o usuário inserir o link, título e imagem do vídeo a ser adicionado e clicar no botão "Enviar", o novo vídeo será inserido e carregará uma página de sucesso.

![apresentacao-alura-play-busca840](https://github.com/CamilaSah/aluraplay-requisicoes/assets/128820692/2f59e72b-925e-4f19-85c1-638eee188474)

![apresentacao-alura-play-add840](https://github.com/CamilaSah/aluraplay-requisicoes/assets/128820692/72f5ae8a-b99e-429f-8c1d-d978eb338fba)


## 📁 Acesso ao projeto
Para poder acessar o projeto, você precisa:
* Baixar a pasta deste projeto.
* Instalar o json-server: simula um servidor local no seu computador.
* Instalar o Node.js: é um ambiente de execução do código Javascript do lado servidor (server side), que permite executar aplicações desenvolvidas com a linguagem sem depender de um navegador.
* Instalar o Live Server: é uma extensão para o Visual Studio Code que cria um servidor local para hospedar seu projeto e atualizar automaticamente a página quando você faz alterações no código. Você pode usar outra aplicação, caso queira.

O passo a passo para conseguir acessar o projeto é:

Caso você ainda não tenha instalado o Node.js e o json-server:
1. Baixar a pasta deste projeto.
2. Entrar no site nodejs.dev e fazer o download no Node.
3. Abrir o projeto no VSCode.
4. Abrir o terminal do VSCode.
5. Clicar em "Terminal" -> “Novo terminal”.
6. Escrever o comando `npm init` para iniciar o npm dentro do projeto.
7. Dar “Enter” em todas as opções.
8. Escrever o comando `npm install -g json-server` para executar a instalação do json-server.

Caso você já tenha instalado o Node.js e o json-server:
1. Baixar a pasta deste projeto.
2. Abrir o projeto no VSCode.
3. Abrir o terminal do VSCode.
4. Clicar em "Terminal" -> “Novo terminal”.
5. Escrever o comando `npx json-server --watch db.json` para iniciar o servidor.
6. Ele vai iniciar o servidor local em uma porta `[PORT_NUMBER]`. Quando você quiser acessar o URL do servidor vai ser localhost:`[PORT_NUMBER]`/videos.
7. Abrir o `index.html` com o Live Server.
<br>
PS¹.: Você pode usar o terminal do Git Bash ao invés do VSCode, caso queira.
PS².: O projeto só irá funcionar se o servidor local estiver sendo executado no terminal do VSCode ou no Git Bash.

## ✔️ Técnicas e tecnologias utilizadas
Técnicas utilizadas:
- ``npm init``: foi utilizado para inicializar o npm dentro do projeto.
- ``npm install -g json-server``: pedido para o npm executar a instalação do json-server para possibilitar o uso dele no projeto.
- ``npx json-server --watch db.json``: iniciar o servidor local.
- ``async/await``: construir funções assíncronas.
- ``try/catch`` e ``throw new Error``: foi utilizado para tratar os erros.
- ``Método fetch()``: é um método assíncrono e tem como parâmetro obrigatório a URL da API.
- ``Método json()``: foi utilizado para converter dados em JSON.
- ``Método forEach()``: foi aplicado para criar um card de cada item da lista que retornar da busca.
- ``Método appendChild()``: foi utilizado para criar os filhos ``li``, que são os cards dos vídeos.
- ``export``: foi utilizada para que a função conectaApi() fosse utilizado em outros arquivos.
- ``import``: foi utilizada para importar a função listaVideos() de um outro arquivo.
- ``Função querySelector()``: faz uma busca do elemento pelo seletor (elemento, classe e id).
- ``Função Math.random`` e ``função Math.floor``: foi utilizado para gerar um número aleatório inteiro de visualizações para a descrição do vídeo.
- ``Data attributes``: foi utilizado para selecionar o elemento da lista.
- ``element.className``: retorna e define o valor do atributo class do elemento especificado.
- ``element.innerHTML``: esta propriedade obtém ou altera qualquer elemento no HTML. Neste caso, o corpo das informações de cada vídeo. 
- ``Template string``: foi utilizado para alterar a descrição de cada card do vídeo de forma dinâmica.
- ``JSON.stringify``: foi utilizado para enviar uma requisição.
- ``requisições GET``: foram criadas para consumir a API da lista de vídeos.
- ``requisição POST``: foi utilizada para salvar dados na API, estruturar requisições do tipo POST enviadas com o fetch API e diferenciar method, headers e body.
- ``Evento submit``: foi utilizado para ser acionado quando o formulário é enviado.
- ``Evento click``: foi utilizado para carregar os vídeos com o termo de busca digitado quando o usuário clicasse no botão de buscar.
- ``while``: foi utilizado para remover todos os outros itens da lista, que já estavam na tela. 
- ``if``: foi utilizado para detectar erros por meio de condicionais.
- ``Node.firstChild``: foi utilizado para retornar o node (nó) do primeiro elemento filho de uma árvore DOM. Neste caso, foi utilizado na condicional em conjunto com o while “enquanto aquela lista tiver um primeiro filho”.
- ``Node.removeChild``: foi utilizado para remover um nó filho do DOM. Neste caso, foi utilizado em conjunto com o while até apagar todos os filhos que a lista tinha.

Tecnologias e ferramentas utilizadas:
- ``Visual Studio Code``: editor de código.
- ``Chrome``: navegador utilizado para teste.
- ``HTML``: fazer a estrutura semântica da página.
- ``CSS``: fazer os estilos da página.
- ``JavaScript``: adicionar o dinamismo e as atualizações de programação, a lógica na página.
- ``Node.JS``: é um ambiente de execução do código Javascript fora do ambiente do navegador.
- ``npm (node package manager)``: é um gerenciador de dependências/pacotes, ou seja, ele é um repositório de código voltado para pacotes do Node.
- ``json-server``: é um pacote npm, que simula um servidor local no nosso computador.
- ``DevTools``: utilizamos a aba “Console”, no qual podemos executar qualquer código JavaScript, além de nos ajudar a desenvolver, a entender o nosso código e ver como os erros são apresentados.
- ``Git``: ferramenta de controle de versão de seu arquivo, projeto ou código. 
- ``GitHub``: plataforma para gerenciar seu código e criar um ambiente de colaboração entre devs (permite compartilhamento de código através da criação de repositórios), utilizando o Git como sistema de controle.
- ``Extensão Live Server``: é uma extensão para o Visual Studio Code que cria um servidor local para hospedar seu projeto e atualizar automaticamente a página quando você faz alterações no código. 

## 📚 Mais informações do curso
Gostou do projeto e quer conhecer mais? Você pode acessar o curso que me ajudou a desenvolver o projeto desde o começo! 
Busque na plataforma da Alura o curso da escola Front-end:
- [JavaScript: criando requisições](https://cursos.alura.com.br/course/javascript-criando-requisicoes).

Esse curso faz parte da formação [Desenvolva aplicações Web com JavaScript](https://cursos.alura.com.br/formacao-javascript-front-end) da Alura
<br>
# Autores

| <img src="https://github.com/CamilaSah/site-pessoal/assets/128820692/bed790ab-3722-4503-8fed-c786e774661b" width="100"><br>[<sub>Camila Sayuri Tokubo</sub>](https://www.linkedin.com/in/camila-tokubo/)|
| :---: |
