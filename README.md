# Quiz App em React

Este é um aplicativo de quiz desenvolvido em React, onde os usuários podem testar seus conhecimentos em programação respondendo a uma série de perguntas.
O projeto foi desenvolvido em Formação Front-end na Udemy.

## Visão Geral

Este projeto consiste em um aplicativo de **quiz interativo** que permite aos usuários escolherem uma categoria de perguntas de programação e responderem a uma série de perguntas. O aplicativo exibe uma mensagem de boas-vindas, permite que os usuários escolham uma categoria de perguntas, exibe perguntas uma por uma, fornece dicas e opções para remover uma opção incorreta, e exibe a pontuação final do usuário após completar todas as perguntas.

# Vídeo do projeto:
![](video/Quiz%20App.mp4)

## Funcionalidades Técnicas:

- Componentização em React:
    O projeto utiliza a biblioteca React para criar uma aplicação frontend modular e componentizada.
    Cada funcionalidade do aplicativo é encapsulada em componentes reutilizáveis, como Welcome, Question, GameOver, e PickCategory. Isto facilita a manutenção do código, tornando-o mais legível e organizado.

- Estado Global com Context API:
    O estado global da aplicação é gerenciado usando a Context API do React.
    O contexto QuizContext e o provedor QuizProvider são utilizados para compartilhar o estado entre os componentes sem a necessidade de passar props manualmente. Isto simplifica a comunicação entre os componentes e evita a propagação excessiva de props.

- Gerenciamento de Estado com useReducer:
    O hook useReducer é utilizado para gerenciar o estado da aplicação de forma mais complexa e estruturada.
    Um reducer (quizReducer) é implementado para processar as ações e atualizar o estado com base nos tipos de ação fornecidos.

- Manipulação Dinâmica do DOM:
    As perguntas e opções são exibidas dinamicamente com base no estado atual do aplicativo.
    O DOM é manipulado condicionalmente para exibir diferentes componentes e conteúdos de acordo com o estágio do jogo (gameStage).

- Interação do Usuário e Feedback Visual:
    O aplicativo oferece interações intuitivas com o usuário, como clicar em botões para iniciar o jogo, selecionar respostas e receber dicas.
    O feedback visual é fornecido ao usuário por meio da alteração de estilos CSS com base nas ações executadas, como selecionar uma resposta correta ou incorreta.

- Utilização de CSS para Estilização:
    O projeto utiliza CSS para estilizar os componentes e criar uma interface de usuário atraente e responsiva.
    Classes CSS são aplicadas dinamicamente para refletir o estado atual do jogo, como destacar opções corretas ou incorretas.

- Reordenamento Aleatório de Perguntas:
    O aplicativo oferece a funcionalidade de reordenar aleatoriamente as perguntas antes do início do jogo.
    Isso é realizado através da ação REORDER_QUESTIONS no reducer, que embaralha a ordem das perguntas no estado global.

- Persistência de Dados e Reinício do Jogo:
    Os dados do jogo, como perguntas, pontuação e estágio atual, são persistidos localmente no estado global.
    Após o término do jogo, os usuários têm a opção de reiniciar o jogo, o que redefine o estado para o inicial.

## Tecnologias Utilizadas
- **React**
- **JavaScript**
- **HTML**
- **CSS**

## Estrutura do Projeto
- src/: Contém o código-fonte do projeto.
- components/: Contém os componentes React utilizados na aplicação.
- context/: Contém o contexto React utilizado para gerenciar o estado do quiz.
- data/: Contém os dados das perguntas em formato JSON.
- App.jsx: Arquivo principal que define a estrutura do aplicativo.
- public/: Contém arquivos públicos, como o arquivo HTML principal.

## Contribuição
Contribuições são bem-vindas! 
Sinta-se à vontade para utilizar, modificar e adaptar este conteúdo, de acordo com as necessidades específicas do seu projeto.

## Autor
- [@RaquelGui](https://www.github.com/RaquelGui)