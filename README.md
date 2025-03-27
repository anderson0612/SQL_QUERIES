# SQL Queries - MySQL

## Este repositório contém uma coleção de consultas SQL desenvolvidas em MySQL para diversos cenários e necessidades. 
## As queries foram organizadas por tipo e aplicação, visando facilitar a compreensão e reutilização.

# Estrutura do Banco de Dados

O banco de dados foi estruturado para suportar os seguintes módulos:

Clientes: Armazena informações sobre os clientes, como nome, endereço, telefone e e-mail.

Fornecedores: Contém dados sobre os fornecedores, incluindo nome, endereço, telefone e informações de contato.

Produtos: Registra os produtos vendidos pela empresa, com descrição, preço, quantidade disponível e código de barras.

Vendas: Armazena informações sobre as transações de venda, incluindo o cliente, os produtos comprados, quantidade e valor total da venda.

# Tabelas do Sistema
## 1. Tabela Clientes:

id_cliente (INT): Identificador único do cliente.

nome_cliente (VARCHAR): Nome completo do cliente.

endereco_cliente (VARCHAR): Endereço completo do cliente.

telefone_cliente (VARCHAR): Número de telefone do cliente.

email_cliente (VARCHAR): E-mail do cliente.

## 2. Tabela Fornecedores:

id_fornecedor (INT): Identificador único do fornecedor.

nome_fornecedor (VARCHAR): Nome completo do fornecedor.

endereco_fornecedor (VARCHAR): Endereço completo do fornecedor.

telefone_fornecedor (VARCHAR): Número de telefone do fornecedor.

email_fornecedor (VARCHAR): E-mail do fornecedor. 

## 3.Tabela Produtos:

id_produto (INT): Identificador único do produto.

descricao_produto (VARCHAR): Descrição do produto.

preco_produto (DECIMAL): Preço unitário do produto.

quantidade_produto (INT): Quantidade disponível em estoque.

codigo_barras_produto (VARCHAR): Código de barras do produto.

## 4. Tabela Vendas:

id_venda (INT): Identificador único da venda.

id_cliente (INT): Identificador do cliente que realizou a compra.

data_venda (DATE): Data da venda.

valor_total (DECIMAL): Valor total da venda.

## 5. Tabela Detalhes_Vendas (Relacionamento entre produtos e vendas):

id_venda (INT): Identificador da venda.

id_produto (INT): Identificador do produto vendido.

quantidade_vendida (INT): Quantidade de produtos vendidos.

preco_unitario (DECIMAL): Preço unitário do produto no momento da venda.

## Funcionalidades

Cadastro de Clientes: Permite o cadastro de novos clientes no sistema.

Cadastro de Fornecedores: Permite o cadastro de novos fornecedores que fornecem os produtos.

Cadastro de Produtos: Permite o cadastro de novos produtos, incluindo preço e quantidade em estoque.

Registro de Vendas: Registra uma venda, associando o cliente aos produtos comprados, com a possibilidade de calcular o valor total da venda.

Consulta de Vendas: Permite visualizar informações sobre as vendas realizadas, produtos vendidos e valores totais.

# Tecnologias Utilizadas

Banco de Dados: SQL (MySQL,).

Ferramenta de Desenvolvimento: Sistema de gerenciamento de banco de dados (MySQL Workbench).


### Estrutura do Projeto

SELECT: Consultas básicas de leitura.

INSERT: Exemplos de inserção de dados.

UPDATE: Consultas para atualização de registros.

DELETE: Excluindo dados de tabelas.

JOIN: Consultas utilizando junção de tabelas.

Funções e Procedimentos: Exemplos de funções e procedimentos armazenados.

