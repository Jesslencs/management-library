
# management-library
Este projeto consiste em um sistema de gerenciamento de biblioteca desenvolvido em Oracle PL/SQL. Ele permite o cadastro de livros, clientes, empréstimos e devoluções, além de fornecer funcionalidades de busca e controle de multas por atraso na devolução.

![modeling library](https://github.com/Jesslencs/management-library/assets/128511563/cb652703-eb8d-4957-968d-5b92767dea02)



# Principais Funcionalidades
 ## 1. Cadastro de Livros

Permite adicionar novos livros à biblioteca, informando título, autor, editora, ano de publicação e quantidade disponível.

 ## 2.Cadastro de Clientes

Permite registrar novos clientes, incluindo nome, endereço, e-mail e telefone.

## 3.Empréstimo de Livros

Permite emprestar livros a clientes, verificando se o livro está disponível e registrando a data de empréstimo.

## 4.Devolução de Livros

Permite que os clientes devolvam os livros emprestados, atualizando a quantidade disponível do livro e calculando multas por atraso, se aplicável.

## 5.Busca de Livros

Permite buscar livros por título, autor ou ano de publicação.
## Funcionamento do Sistema
O sistema é composto por três partes principais: a tabela library_books para armazenar informações sobre os livros, a tabela library_clients para armazenar informações sobre os clientes e a tabela library_loan para controlar os empréstimos.

Para cada operação, como adicionar um livro ou emprestar um livro a um cliente, há uma procedure correspondente na package library_package. Essas procedures realizam as operações necessárias e podem retornar mensagens de sucesso ou erro.

Além disso, o sistema inclui triggers para aplicar multas automaticamente quando um livro não é devolvido dentro do prazo.

# English version

This project is a library management system developed in Oracle PL/SQL. It allows for managing books, clients, loans, and returns, including search functionality and late return penalty tracking.

# Key Features
## Book Management: 
Add new books with title, author, publisher, publication year, and quantity available.
## Client Management:
Register clients with name, address, email, and telephone.
## Book Loan: 
Enable clients to borrow books, checking availability and recording loan dates.
## Book Return: 
Allow clients to return books, updating availability and calculating late penalties if applicable.
## Book Search:
Search for books by title, author, or publication year.
# System Overview
The system uses tables for storing book and client information, with procedures in the library_package for operations like adding books and lending books to clients. Triggers are used to apply penalties for late returns.
