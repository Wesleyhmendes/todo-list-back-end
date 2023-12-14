# Docker Todo List

Neste projeto, as seguintes tarefas foram feitas:
1. Conteinerizar aplicações;
2. Criar uma conexão entre elas;
3. Orquestrar seu funcionamento.

Temos uma aplicação full-stack: um aplicativo de tarefas! Esta aplicação foi conteinerizada graças ao desenvolvimento dos arquivos de configuração para cada frente específica: `Front-end` e `Back-end`.
Os arquivos principais do projeto estão na pasta `docker`, na raiz do projeto. Nela estão contidos:

1. Pasta `docker-commands`: onde ficarão os comandos exigidos pelos requisitos;
   - **⚠️ Importante: você deve assumir que essa é a pasta raiz para os comandos.**
   - Por exemplo, se você precisa referenciar um caminho em um comando, você deve assumir que sua pasta raiz esta partindo de `./docker`.
2. Pasta `todo-app`: onde fica a nossa **pseudo-aplicação**, que servirá como base para nossos `Dockerfile`s e `Compose`;

## 🚀 Começando

> - ⚠️ É necessário ter a versão Node 16.14 ou superior instalada localmente.

<br />

<details>
<summary><strong> ⚠️ Configurações mínimas para execução do projeto</strong></summary><br />

Na sua máquina você deve ter:

 - Sistema Operacional Distribuição Unix
 - Node versão 16
 - Docker
 - Docker-compose versão >=1.29.2

➡️ O `node` deve ter versão igual ou superior à `16.14.0 LTS`:
  - Para instalar o nvm, [acesse esse link](https://github.com/nvm-sh/nvm#installing-and-updating);
  - Rode os comandos abaixo para instalar a versão correta de `node` e usá-la:
    - `nvm install 16.14 --lts`
    - `nvm use 16.14`
    - `nvm alias default 16.14`

➡️ O`docker-compose` deve ter versão igual ou superior à`ˆ1.29.2`:
  * Verifique no Course no dia `Orquestrando Containers com Docker Compose` como instalar corretamente.
  * Caso necessário, acesse o [link da documentação oficial com passos para desinstalar](https://docs.docker.com/compose/install/#uninstallation) a versão atualmente instalada.

</details>

<details>
  <summary><strong>🔧 Instalação</strong></summary>
<br />
  
1. Clone o repositório
  * `git clone git@github.com:Wesleyhmendes/all-for-one-back-end.git`.
  * Entre na pasta do repositório que você acabou de clonar:
    * `cd all-for-one-back-end`

2. Instale as dependências [**Caso existam**]
  * `npm install`

3. Crie uma branch a partir da branch `master`
  * Verifique que você está na branch `master`
    * Exemplo: `git branch`
  * Se não estiver, mude para a branch `master`
    * Exemplo: `git checkout master`
  * Agora crie uma branch com o nome desejado

<br />
</details>

<br />

<details>
  <summary><strong>📋 Requisitos</strong></summary>
<br />

**1 - Crie um container em modo interativo, sem rodá-lo, nomeando-o como `01container` e utilizando a imagem `alpine` na versão `3.12`**


**2 - Inicie o container `01container`**


**3 - Liste os containers filtrando pelo nome `01container`**


**4 - Execute o comando `cat /etc/os-release` no container `01container` sem se acoplar a ele**


**5 - Remova o container `01container`**


**6 - Faça o download da imagem `nginx` com a versão `1.21.3-alpine` sem criar ou rodar um container**


**7 - Rode um novo container com a imagem  `nginx` com a versão `1.21.3-alpine` em segundo plano nomeando-o como `02images` e mapeando sua porta padrão de acesso para porta `3000` do sistema hospedeiro**


**8 - Pare o container `02images` que está em andamento**


**9 - Gere uma build a partir do Dockerfile do `back-end` do `todo-app` nomeando a imagem para `todobackend`**


**10 - Gere uma build a partir do Dockerfile do `front-end` do `todo-app` nomeando a imagem para `todofrontend`**


**11 - Gere uma build a partir do Dockerfile dos `testes` do `todo-app` nomeando a imagem para `todotests`**

<br />

### Requisito bônus do projeto

### Docker-compose
**12 - Suba uma orquestração em segundo plano com o docker-compose de forma que `backend`, `frontend` e `tests` consigam se comunicar**

</details>

## 🛠️ Construído com

Mencione as ferramentas que você usou para criar seu projeto

* [npm](https://www.npmjs.com/) - Gerente de Dependência

## 📌 Versão

Nós usamos [Docker](https://www.docker.com/) para controle de versão.

## ✒️ Autores

* **Wesley Mendes** - *Trabalho Inicial* - [Wesley Mendes](https://github.com/Wesleyhmendes)
