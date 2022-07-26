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

- [x] [step-1:](https://github.com/WagnerCOliveira/dotdigital/tree/step1)
  - Serviços comuns a todas as aplicações (db, proxy etc);
- [x] [step-2:](https://github.com/WagnerCOliveira/dotdigital/tree/step2)
  - Aplicação 1 sem persistência de dados;
- [x] [step-3:](https://github.com/WagnerCOliveira/dotdigital/tree/step3)
  - Aplicação 2 sem persistência de dados;
- [x] [step-4:](https://github.com/WagnerCOliveira/dotdigital/tree/step4)
  - Aplique a persistência de dados para as duas aplicações. A organização em branches deve, por exemplo, possibilitar o uso das duas aplicações de forma efêmera no branch "step-3".

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