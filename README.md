#  API de Categorias

API REST desenvolvida em Java com Spring Boot para gerenciamento de categorias.

O projeto implementa operações básicas de CRUD seguindo boas práticas de organização em camadas (Controller, Repository e DTOs).

---

##  Funcionalidades

* ✅ Cadastro de categorias
* ✅ Listagem de categorias
* ✅ Atualização de categorias
* ✅ Exclusão de categorias

---

##  Tecnologias utilizadas

* Java
* Spring Boot
* Spring Data JPA
* Maven
* H2 / Banco configurável via `application.properties`

---

##  Estrutura do projeto

```
src/main/java/br/com/fiap/API/
├── controller/
│   └── CategoriaController.java
├── categoria/
│   ├── Categoria.java
│   ├── CategoriaRepository.java
│   ├── DadosCadastroCategoria.java
│   ├── DadosAtualizarCategoria.java
│   └── DadosDetalhamentoCategoria.java
└── ApiApplication.java
```

---

##  Como rodar o projeto

### 1. Clone o repositório

```bash
git clone https://github.com/<seu-usuario>/<nome-repo>.git
cd <nome-repo>
```

### 2. Execute a aplicação

Se estiver usando Maven Wrapper:

```bash
./mvnw spring-boot:run
```

Ou no Windows:

```bash
mvnw.cmd spring-boot:run
```

---

## Configuração

As configurações estão no arquivo:

```
src/main/resources/application.properties
```

Você pode alterar:

* Porta da aplicação
* Configuração do banco de dados

---

##  Endpoints

###  Categoria

| Método | Rota             | Descrição                 |
| ------ | ---------------- | ------------------------- |
| GET    | /categorias      | Lista todas as categorias |
| POST   | /categorias      | Cria uma nova categoria   |
| PUT    | /categorias      | Atualiza uma categoria    |
| DELETE | /categorias/{id} | Remove uma categoria      |

---

##  Testes

Para rodar os testes:

```bash
./mvnw test
```

---

##  Licença

Este projeto é de uso acadêmico.

---

## 👨‍💻 Autor

Pedro Chamusca
Projeto desenvolvido para fins de estudo em Sistemas de Informação (FIAP).
