# 🛒 Base de Dados - Loja (MySQL)

Este repositório contém o script SQL (`BdeD.sql`) com os comandos DDL (Data Definition Language) para a criação, modificação e gestão da base de dados relacional de um sistema de **Loja**.

## 📊 Estrutura da Base de Dados

A base de dados é composta por 3 tabelas principais com relações entre si:

1. **`cliente`**: Armazena as informações dos clientes da loja.
   - `id`: Identificador único (Primary Key, Auto Increment).
   - `nome`: Nome do cliente.
   - `email`: Endereço de e-mail (Único).

2. **`produto`**: Regista os produtos disponíveis na loja.
   - `id`: Identificador único (Primary Key, Auto Increment).
   - `nome`: Nome do produto.
   - `preco`: Preço do produto (Formato `DECIMAL(5,2)`).

3. **`pedido`**: Associa os clientes aos produtos adquiridos.
   - `id`: Identificador único (Primary Key, Auto Increment).
   - `data_pedido`: Data de realização da encomenda.
   - `cliente_id`: Chave estrangeira (`FOREIGN KEY`) a referenciar a tabela `cliente`.
   - `produto_id`: Chave estrangeira (`FOREIGN KEY`) a referenciar a tabela `produto`.

---

## 🛠️ Conteúdo do Script (`BdeD.sql`)

O ficheiro inclui comandos para:
- **Criação da Base de Dados**: `CREATE DATABASE loja;`
- **Criação de Tabelas**: Definição das tabelas `cliente`, `produto` e `pedido` com restrições e relacionamentos.
- **Alteração de Estrutura (`ALTER TABLE`)**: Exemplos de como adicionar, renomear, modificar e remover colunas na tabela `cliente`.
- **Consultas Básicas**: Seleção de dados (`SELECT`).
- **Remoção de Estruturas**: Comandos de eliminação (`DROP TABLE` e `DROP DATABASE`).

---

## 🚀 Como Executar o Script

### Pré-requisitos
- Ter o **MySQL Server** instalado.
- Um cliente de base de dados como **MySQL Workbench**, **DBeaver** ou a CLI do MySQL.

### Passo a Passo

1. Clone o repositório para a sua máquina:
   ```bash
   git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
