# Customer API

<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Java Version](https://img.shields.io/badge/Java-21%2B-blue)](https://www.java.com/)
[![GitHub repo size](https://img.shields.io/github/repo-size/marllonmendez/stories?color=blue)]()
[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/marllonmendez/stories?color=blue)]()

[![Sprinb Boot](https://img.shields.io/badge/Spring_Boot-F2F4F9?style=for-the-badge&logo=spring-boot)](https://spring.io/projects/spring-boot)
[![Hinernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white)](https://hibernate.org/)
[![Maven](https://img.shields.io/badge/apache_maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)](https://maven.apache.org/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)](postgresql.org/)


</div>

## Sobre
API criada para ser utilizado no [Customer APP](https://github.com/marllonmendez/customer-app)

## Funcionalidades

- Cadastro de Clientes;
- Listagem de CLientes;
- Busca de Clientes.

## Execução
<h4>1. Instalação de Dependências:</h4>

```bash
mvn install
```
Este comando irá baixar as dependências do projeto e construir o projeto. Ele executa as fases `compile`, `test`, e `package` do ciclo de vida do Maven.

<h4>2. Configuração do Banco de Dados PostgreSQL:</h4>
 
**Observação:**
O PostgreSQL deve sempre estar aberto. Caso contrário, a API encerrará sua execução, informando que não encontrou o banco de dados.

- Instale o [PostgreSQL](https://www.postgresql.org/download/)
- Configure a senha do banco de dados no arquivo `src/main/resources/application.properties` na propriedade `spring.datasource.password`. Esta senha deve corresponder a mesma configurada no PostgreSQL.
- Configure o usuário do banco de dados no arquivo `src/main/resources/application.properties` na propriedade `spring.datasource.username`. Este usuário deve corresponder o mesmo configurado no PostgreSQL.
- Abra o PostgreSQL e crie um **Banco de Dados** chamado `customerSystem` somente assim a aplicação fara a conexão com o database ou se preferir mude o nome/porta no arquivo `src/main/resources/application.properties` na propriedade `spring.datasource.url`.

<h4>3. Execução do Projeto:</h4>

```bash
mvn spring-boot:run
```

- Se quiser parar de executar aperte as teclas ```ctrl + c```
- Se no terminal perguntar ``Deseja finalizar o arquivo em lotes (S/N)?`` responda ``S``


<h4>4. Configuração de requisições HTTP (Para Testes):</h4>

- Instale o [Insominia](https://insomnia.rest/)
- configure e importe dentro do Insominia o projeto [Customer API](https://drive.google.com/drive/folders/1Yqjj-nLGlGoynUlFK0H-QcyBVTQRYTxb?usp=sharing)

<h4>5. Limpeza do Projeto:</h4>

```bash
mvn clean
```

Este comando remove os arquivos gerados durante a compilação e construção do projeto. Isso é útil se você deseja limpar o projeto antes de construir novamente.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).
