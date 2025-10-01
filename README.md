# Implementação de Banco de Dados PostgreSQL na Nuvem

## Contextualização
Uma equipe de desenvolvimento de software precisa implementar uma solução de banco de dados na nuvem para atender às necessidades de um projeto corporativo.  
A escolha da empresa foi utilizar o serviço **Render** para hospedar um banco **PostgreSQL**, que permitirá maior escalabilidade, segurança e facilidade de integração com outras ferramentas.

Neste cenário, o time deve estruturar a base de dados, aplicar boas práticas de modelagem, realizar inserções em massa e configurar permissões de acesso, garantindo que a solução seja funcional e segura.

---

## Desafio
Como parte da equipe de desenvolvimento, você deverá implementar e configurar um banco de dados PostgreSQL na nuvem no **Render**, além de executar tarefas de manipulação de dados e controle de usuários.

As etapas do desafio incluem:

---

### 1. Criação do Banco de Dados
- Criar um banco chamado **col-seunome**, onde `seunome` é substituído pelo nome do aluno.
- Conectar o banco ao **DBeaver** para gerenciar e executar os scripts.

---

### 2. Criação da Tabela `alunos`
Criar uma tabela chamada **alunos** com os seguintes campos:
- id INT, cpf VARCHAR(18), nome VARCHAR(80), endereco VARCHAR(80), telefone VARCHAR(20), email VARCHAR(20), uf CHAR(2)
- Todos os campos devem ser **NOT NULL**.  
- O campo **id** deve ser a **chave primária**.  
- Os campos devem seguir o padrão **nomedocampo_nomedatabela** (ex.: `id_aluno`).

---

### 3. Manipulação de Dados
- Criar um **INSERT** com **100 registros** (os dados podem ser gerados com auxílio de uma IA generativa).  
- Atualizar o campo `uf_aluno` de todos os registros com `id_aluno > 70` para **SC**.  
- Excluir todos os registros com `id_aluno > 90`.  

---

### 4. Consultas
- Realizar uma consulta que exiba os nomes de todos os alunos cujo `nome_aluno` começa com a letra **F**.  
- Criar uma **VIEW** chamada `pesquisa` que execute essa consulta.  

---

### 5. Gerenciamento de Usuários
- Criar o usuário **felippe** com senha **54321**.  
- Conceder permissão ao usuário **felippe** para executar a **view pesquisa**.  

---

## Entrega
Os alunos deverão enviar:
1. Os **scripts SQL** de cada ação realizada.  
2. O **host do banco** e o **nome do banco** para validação.  

---

## Resultados Esperados
- Banco de dados **col-seunome** corretamente criado e acessível pelo Render e DBeaver.  
- Tabela **aluno** criada conforme as especificações, respeitando o padrão de nomenclatura.  
- Inserção em massa de **100 registros** concluída com sucesso.  
- Atualização correta do campo `uf_aluno` para registros com `id_aluno > 70`.  
- Exclusão de registros com `id_aluno > 90` realizada corretamente.  
- Consulta que retorna os alunos cujo nome começa com **F** implementada com sucesso.  
- **View pesquisa** criada corretamente a partir da consulta.  
- Usuário **felippe** criado com senha definida e permissões de execução atribuídas à view.  
- Scripts, host e nome do banco entregues dentro do prazo estabelecido.  
