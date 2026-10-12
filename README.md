# 🥟 Baozi Store - API RESTful

API RESTful desenvolvida em Java e Spring Boot para gestão de clientes, produtos e pedidos da loja fictícia **Baozi Store**. Este projeto foi desenvolvido como Atividade Prática da disciplina de **Desenvolvimento Web Back End**.

---

## 📌 Descrição da Situação Fictícia

A **Baozi Store** é uma pequena loja especializada na venda de pão chinês (*Baozi*). Para otimizar a organização e gestão do negócio, foi implementada esta API backend para controlar os cadastros e operações de clientes, produtos e pedidos.

* **Cliente:** `CamilleBarbosadosSantos5442792`
* **Produto:** `Baozi Tradicional` (vendido por unidade)
* **Pedido:** Registro de compra de 5 unidades do produto pelo cliente cadastrado.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Java 17+
* **Framework:** Spring Boot 3+
* **Persistência de Dados:** Spring Data JPA
* **Banco de Dados:** H2 Database (Banco em memória)
* **Gerenciador de Dependências:** Maven
* **Arquitetura:** Padrão MVC (Model-View-Controller)
* **Testes de Endpoints:** Postman

---

## 🏗️ Estrutura do Projeto

O projeto segue a arquitetura em camadas padrão do Spring Boot:

```text
src/main/java/com/baozi/store/
├── controller/       # Camada de exposição dos Endpoints REST
│   ├── ClienteController.java
│   ├── PedidoController.java
│   └── ProdutoController.java
├── model/            # Entidades do JPA (Tabelas do Banco de Dados)
│   ├── Cliente.java
│   ├── Pedido.java
│   └── Produto.java
├── repository/       # Interfaces de acesso aos dados (CRUD JPA)
│   ├── ClienteRepository.java
│   ├── PedidoRepository.java
│   └── ProdutoRepository.java
└── StoreApplication.java  # Classe Principal de Execução


