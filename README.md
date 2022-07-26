# Instalação e Configuração GItea Docker Swarm

## Projeto de SCM para os codigos de infra estrutura.


Tabela de conteúdos
=================
<!--ts-->      
   * [Questão](#questão)
   * [Tecnologias](#-tecnologias-utilizadas)
   * [Contribuição](#contribuição)
   * [Autor](#autor)
   * [Licença](#licença)
<!--te-->


### Questão

Crie um repositório público (github por exemplo) contendo o passo-a-passo no formato de branches (para que seja possível fazer checkout para o passo desejado) da composição de um arquivo docker-compose, com os seguintes itens, nesta ordem:

- [x] step-3: 
  - Aplicação 2 sem persistência de dados;

#### Criação .env
Para o docker compose reconhecer as configurações de banco de dados é necessário ter o arquivo **.env** na raiz do projeto com as seguintes variaveis. 
> Obs.: Colocar ums senha para o banco de dados e outra para o root do mysql.

~~~bash
USER_UID=1000
USER_GID=1000
GITEA__database__DB_TYPE=mysql
GITEA__database__HOST=db
GITEA__database__NAME=gitea
GITEA__database__USER=gitea
GITEA__database__PASSWD=INSIRA_SENHA_PARA_BANCO_GITEA
MYSQL_ROOT_PASSWORD=INSIRA_SENHA_PARA_ROOT_MYSQL
MYSQL_USER=gitea
MYSQL_PASSWORD=INSIRA_SENHA_PARA_BANCO_GITEA
MYSQL_DATABASE=gitea
~~~ 

### 🛠 Tecnologias Utilizadas

As seguintes ferramentas foram usadas na construção do projeto:

- [Git](https://git-scm.com/)
- [Docker 20.10.12](https://docs.docker.com/engine/)
- [Docker Compose 1.29.2](https://docs.docker.com/compose/)
- [Gitea 1.16.4](https://docs.gitea.io/en-us/)
- [Mysql 8](https://dev.mysql.com/doc/)

### Contribuição

* [Wagner C Oliveira](https://www.wagneroliveira.eti.br)

### Autor

* [Wagner C Oliveira](https://www.wagneroliveira.eti.br)

### Licença

* [GNU General Public License (GPL)](https://www.gnu.org/licenses/gpl-3.0.html)