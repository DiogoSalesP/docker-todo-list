# :construction: README customizado em construção ! :construction:
<!-- Olá, Tryber!
Esse é apenas um arquivo inicial para o README do seu projeto no qual você pode customizar e reutilizar todas as vezes que for executar o trybe-publisher.

Para deixá-lo com a sua cara, basta alterar o seguinte arquivo da sua máquina: ~/.student-repo-publisher/custom/_NEW_README.md

É essencial que você preencha esse documento por conta própria, ok?
Não deixe de usar nossas dicas de escrita de README de projetos, e deixe sua criatividade brilhar!
:warning: IMPORTANTE: você precisa deixar nítido:
- quais arquivos/pastas foram desenvolvidos por você; 
- quais arquivos/pastas foram desenvolvidos por outra pessoa estudante;
- quais arquivos/pastas foram desenvolvidos pela Trybe.
-->

  <summary><strong>👨‍💻 O que deverá ser desenvolvido</strong></summary><br />

Neste projeto você irá:

1. **_Conteinerizar_** aplicações;
2. Criar uma conexão entre elas;
3. Orquestrar seu funcionamento.

Temos [uma aplicação full-stack](docker/todo-app) neste repositório: um **aplicativo de tarefas**! Esta aplicação precisa ser conteinerizada para funcionar. Você deverá desenvolver os arquivos de configuração para cada frente específica: `Front-end`, `Back-end` e, no nosso caso, para um aplicativo de `teste` que valida se as aplicações estão se comunicando.

---

Você deverá criar as imagens para as aplicações e configurar essas imagens com o `docker-compose`.

Para isto, você irá utilizar uma série de comandos do `docker` com diferentes níveis de complexidade.

Cada comando deverá ser escrito em seu próprio arquivo.

Para isto, siga os seguintes passos:

1. Leia o requisito e crie um arquivo chamado `commandN.dc` no diretório `docker-commands`, onde `N` é o número do requisito. Por exemplo:

    ```text
    Requisito 1: ./docker/docker-commands/command01.dc
    Requisito 2: ./docker/docker-commands/command02.dc
    Requisito 3: ./docker/docker-commands/command03.dc
    ```
    **⚠️ É muito importante que os seus arquivos tenham exatamente estes nomes! ⚠️**


2. Escreva neste arquivo o comando do CLI *(Interface de Linha de Comando)* do Docker que resolve o requisito. Um exemplo de como vai ficar seu arquivo:

    ```dc
    docker network inspect bridge
    ```

---

Os arquivos principais do projeto estão na pasta `docker`, na raiz do projeto. Nela estão contidos:

1. Pasta `docker-commands`: onde ficarão os comandos exigidos pelos requisitos;
   - **⚠️ Importante: você deve assumir que essa é a pasta raiz para os comandos.**
   - Por exemplo, se você precisa referenciar um caminho em um comando, você deve assumir que sua pasta raiz esta partindo de `./docker`.
2. Pasta `todo-app`: onde fica a nossa **pseudo-aplicação**, que servirá como base para nossos `Dockerfile`s e `Compose`;
   - **⚠️ Essa aplicação conta com um [**README.md**](./docker/todo-app/README.md) próprio, que pode ser usado como referência na criação dos `dockerfiles` e do `docker-compose.yml`!**

Quando for necessário fazer a orquestração das aplicações, o arquivo `docker-compose.yml` deverá ser criado na pasta `./docker`. conforme o arquivo de exemplo [`docker/docker-compose.yml.example`](docker/docker-compose.yml.example).
