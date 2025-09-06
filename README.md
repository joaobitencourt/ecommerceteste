[![Status](https://img.shields.io/badge/Status-Em%20Estudo-ff69b4)](https://github.com/seu-usuario/seu-repositorio)
[![Tipo](https://img.shields.io/badge/Tipo-Repositório%20de%20Estudos-blue)](https://github.com/seu-usuario/seu-repositorio)
# Desafio Técnico: Desenvolvedor Pleno

## 🎯 Objetivo
Construir um sistema de gerenciamento de pedidos e produtos para um e-commerce, garantindo:
- Autenticação segura com JWT
- CRUD completo de produtos
- Gerenciamento de pedidos com regras específicas
- Otimização de queries SQL para melhor performance

## 📌 Requisitos

### 🔑 Autenticação
- Implementar JWT para autenticação
- Criar dois perfis de usuário:
    - **ADMIN** → Pode criar, atualizar e deletar produtos
    - **USER** → Pode criar pedidos e visualizar produtos

### ⚙️ Funcionalidades

#### Produtos
Criar um CRUD completo para produtos com os seguintes campos:
- ID (UUID)
- Nome
- Descrição
- Preço
- Categoria
- Quantidade em estoque
- Data de criação
- Data de atualização

#### Pedidos
- Um USER pode criar um pedido contendo múltiplos produtos
- O pedido deve iniciar com o status **PENDENTE**
- Criar uma rota para realizar o pagamento do pedido
- Atualizar o estoque dos produtos apenas após o pagamento do pedido
- Se algum produto do pedido não tiver estoque disponível, o pedido deve ser cancelado automaticamente, e o usuário informado
- O valor total do pedido deve ser calculado dinamicamente com base no preço atual dos produtos
- Criar um endpoint para listar pedidos do usuário autenticado

### 📊 Consultas SQL Otimizadas
Criar endpoints que executem consultas otimizadas no MySQL:
- Top 5 usuários que mais compraram
- Ticket médio dos pedidos de cada usuário
- Valor total faturado no mês

## 🛠 Tecnologias
- Java 17+
- Spring Boot (Security, Data, Web, etc.)
- MySQL
- Spring Data JPA

## 📥 Como Entregar
- Subir o código em um repositório público no GitHub
- Incluir um dump do banco de dados MySQL
- Criar um README documentando as instruções para rodar o projeto