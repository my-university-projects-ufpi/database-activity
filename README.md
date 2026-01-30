# 🗄️ Projeto de Banco de Dados – Sistema Empresarial

Este repositório contém um trabalho acadêmico desenvolvido para a disciplina de **Banco de Dados**, com foco na modelagem, implementação e validação de um sistema de informações para uma empresa.

O projeto contempla desde a modelagem conceitual até a implementação física do banco de dados em **MySQL**, além de relatórios e documentos avaliativos.

---

## 📌 Sobre o Projeto

O objetivo principal deste trabalho é representar, por meio de um banco de dados relacional, o funcionamento de uma empresa, abrangendo áreas como:

* Gestão de funcionários
* Controle de clientes
* Cadastro de fornecedores
* Registro de produtos
* Gerenciamento de pedidos
* Controle de pagamentos
* Registro de ponto

O sistema foi projetado utilizando boas práticas de modelagem relacional, com aplicação de chaves primárias, estrangeiras e normalização.

---

## 📂 Estrutura do Repositório

```
Banco-de-Dados-Empresa
│
├── ProvaEscrita03 BD-20211d.pdf
├── Resenha dissertativa.odt
├── empresa.mwb
├── empresa.mwb.bak
├── empresaSQL.sql
├── empresadiagrama.png
└── .gitattributes
```

---

## 📁 Descrição dos Arquivos

### 📄 ProvaEscrita03 BD-20211d.pdf

Documento referente à avaliação escrita da disciplina.

Contém questões teóricas sobre:

* Modelagem de dados
* Normalização
* SQL
* Conceitos fundamentais de banco de dados

---

### 📄 Resenha dissertativa.odt

Arquivo contendo uma resenha dissertativa relacionada aos temas estudados na disciplina.

Aborda conceitos como:

* Importância dos bancos de dados
* Gerenciamento da informação
* Sistemas de informação

---

### 📄 empresa.mwb

Arquivo do **MySQL Workbench** contendo o modelo do banco de dados.

Inclui:

* Diagrama entidade-relacionamento
* Tabelas
* Relacionamentos
* Restrições

Este arquivo permite editar e visualizar o projeto graficamente.

---

### 📄 empresa.mwb.bak

Arquivo de backup do modelo criado no MySQL Workbench.

Utilizado para recuperação em caso de perda ou corrupção do arquivo principal.

---

### 📄 empresaSQL.sql

Script SQL responsável pela criação e alimentação do banco de dados.

Contém:

* Criação do schema `empresa`
* Definição das tabelas
* Chaves primárias e estrangeiras
* Índices
* Inserção de dados
* Consultas de validação

Este arquivo permite recriar todo o banco de dados automaticamente.

---

### 📄 empresadiagrama.png

Imagem do diagrama gerado pelo MySQL Workbench.

Representa visualmente:

* Entidades
* Relacionamentos
* Cardinalidades
* Estrutura do banco

Facilita a compreensão do modelo lógico.

---

## 🗃️ Modelo do Banco de Dados

O banco de dados foi denominado **`empresa`** e possui as seguintes principais entidades:

### 🏢 Empresa

* Armazena dados da empresa
* Identificada pelo CNPJ

### 👨‍💼 Funcionário

* Dados dos colaboradores
* Cargo, salário, contato
* Relacionado à empresa

### 👥 Cliente

* Informações dos clientes
* Dados pessoais e contato

### 🏭 Fornecedor

* Cadastro dos fornecedores
* Responsáveis pelos produtos

### 📦 Produto

* Informações dos produtos
* Relacionado ao fornecedor

### 📝 Pedido à Vista

* Registro de vendas à vista
* Relacionado ao cliente e empresa

### 📝 Pedido a Prazo

* Registro de vendas parceladas
* Controle de parcelas

### 💳 Parcela Paga

* Controle de pagamentos
* Vinculada ao pedido a prazo

### ⏱️ Ponto Batido

* Registro de entrada e saída dos funcionários

### 🔗 Tabelas Associativas

* `produto_has_pedidoAVista`
* `produto_has_pedidoAPrazo`

Responsáveis por representar o relacionamento muitos-para-muitos entre pedidos e produtos.

---

## 🎯 Objetivos do Trabalho

* Aplicar conceitos de modelagem relacional
* Desenvolver diagramas ER
* Implementar banco em MySQL
* Criar scripts SQL completos
* Inserir dados para testes
* Realizar consultas
* Validar integridade referencial

---

## 🛠️ Tecnologias Utilizadas

* MySQL
* MySQL Workbench
* SQL
* LibreOffice / OpenOffice
* PDF

---

## 📚 Aprendizados

Com este projeto, foi possível:

* Compreender a importância da modelagem de dados
* Trabalhar com relacionamentos entre tabelas
* Aplicar chaves estrangeiras
* Criar consultas SQL
* Garantir integridade dos dados
* Utilizar ferramentas gráficas para banco de dados

---

## 🚀 Como Executar o Projeto

### Requisitos

* MySQL Server
* MySQL Workbench (opcional)

### Passos

1. Abra o MySQL
2. Crie uma conexão
3. Execute o arquivo `empresaSQL.sql`
4. O banco será criado automaticamente
5. Utilize os comandos `SELECT` para validação

---

## 📊 Consultas de Teste

O script já inclui comandos como:

```sql
SELECT * FROM empresa.cliente;
SELECT * FROM empresa.funcionario;
SELECT * FROM empresa.produto;
```

Essas consultas permitem verificar se os dados foram inseridos corretamente.

---
