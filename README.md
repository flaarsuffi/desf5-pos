
# ProductsSpring API

Projeto desenvolvido como desafio final do Bootcamp de Arquiteto(a) de Software.

Este projeto consiste na criação de uma API RESTful para gerenciamento de produtos, seguindo o padrão arquitetural MVC (Model-View-Controller), utilizando Java, Spring Boot e MySQL como banco de dados.

---

## Tecnologias utilizadas

- Java 17
- Spring Boot
- Spring Web
- Spring Data JPA
- MySQL
- Maven

---

## Estrutura de Pastas

```
src/main/java/com/flaarsuffi/productsapi/
├── controller/      # Controladores das requisições HTTP
├── model/           # Entidades de domínio
├── repository/      # Interfaces de acesso a dados
├── service/         # Lógica de negócios
└── ProductsSpringApplication.java  # Classe principal

src/main/resources/
└── application.properties  # Configurações da aplicação
```

---

## Como rodar o projeto

### Pré-requisitos:

- Java 17 instalado
- MySQL instalado e rodando
- Maven instalado

### Passos:

1. Clone o repositório:
   ```bash
   git clone https://github.com/flaarsuffi/desf5-pos.git
   ```

2. Acesse a pasta do projeto:
   ```bash
   cd desf5-pos
   ```

3. Configure o banco de dados:

   - Crie um banco no MySQL:
     ```sql
     CREATE DATABASE productsdb;
     ```

   - Altere o arquivo `src/main/resources/application.properties` com seu usuário e senha do MySQL:
     ```properties
     spring.datasource.username=SEU_USUARIO
     spring.datasource.password=SUA_SENHA
     ```

4. Compile e rode o projeto:

   ```bash
   ./mvnw spring-boot:run
   ```

5. A API estará disponível em:
   ```
   http://localhost:8080/products
   ```

---

## Endpoints disponíveis

- `GET /products` - Lista todos os produtos
- `GET /products/{id}` - Busca produto por ID
- `GET /products/name/{name}` - Busca produtos pelo nome
- `GET /products/count` - Retorna a quantidade de produtos cadastrados
- `POST /products` - Cadastra um novo produto
- `DELETE /products/{id}` - Remove um produto

---

## Autor

Desenvolvido por **Flavia Arsuffi** ✨
