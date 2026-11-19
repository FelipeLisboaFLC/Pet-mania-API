# 🐾 Pet Mania API

API REST desenvolvida em Java com Spring Boot para o gerenciamento de animais disponíveis para adoção. O projeto faz parte do desafio **Pet Mania**, cujo objetivo é identificar e corrigir problemas em uma aplicação Back-end, garantindo o funcionamento das operações de cadastro e gerenciamento de animais.

## 🎯 Objetivo do Projeto

O objetivo é desenvolver e corrigir uma API que permita cadastrar, consultar e atualizar, utilizando uma aplicação Front-end para interagir com os dados e o Postman para validar os endpoints.

## 🚀 Funcionalidades

- [x] Cadastrar animais.
- [x] Listar todos os animais.
- [x] Buscar animal pelo ID.
- [x] Atualizar informações de um animal.
- [x] Integração com banco de dados MySQL.
- [x] Integração com o Front-end Pet Mania.

## 🛠️ Tecnologias Utilizadas

- **Java 25** — Linguagem de programação.
- **Spring Boot 4.1.2** — Framework para desenvolvimento da API.
- **Spring Data JPA** — Persistência e gerenciamento dos dados.
- **MySQL** — Banco de dados relacional.
- **Maven** — Gerenciamento de dependências.
- **Postman** — Testes dos endpoints REST.
- **HTML, CSS e JavaScript** — Interface Front-end.

## 📂 Estrutura do Projeto

```text
Pet-mania-API/
├── src/
│   ├── main/
│   │   ├── java/com/dt2/petmania/
│   │   │   ├── controllers/
│   │   │   │   └── PetController.java
│   │   │   ├── entities/
│   │   │   │   ├── enums/
│   │   │   │   └── Pet.java
│   │   │   ├── repositories/
│   │   │   │   └── PetRepository.java
│   │   │   └── PetManiaApplication.java
│   │   └── resources/
│   │       ├── static/
│   │       │   └── index.html
│   │       └── application.properties
│   └── test/
├── pom.xml
└── README.md
```

## 🐶 Dados dos Animais

O sistema permite armazenar as seguintes informações:

| Campo | Descrição |
|---|---|
| id | Identificador do animal |
| nome | Nome do animal |
| especie | Espécie |
| raca | Raça |
| idade | Idade em anos |
| sexo | Macho ou Fêmea |
| porte | Pequeno, Médio ou Grande |
| personalidade | Características do animal |
| foto | URL da imagem |
| disponivel | Disponibilidade para adoção |

## 🔗 Endpoints da API

A API utiliza o endereço base:

```http
http://localhost:8080/api/pets
```

| Método | Endpoint | Descrição |
|---|---|---|
| GET | `/api/pets` | Lista todos os animais |
| GET | `/api/pets/{id}` | Busca um animal pelo ID |
| POST | `/api/pets` | Cadastra um novo animal |
| PUT | `/api/pets/{id}` | Atualiza um animal |
| DELETE | `/api/pets/{id}` | Exclui um animal |

## ⚙️ Como Executar o Projeto

### 1. Pré-requisitos

Antes de começar, tenha instalado:

- Java JDK 25.
- MySQL.
- Uma IDE, como IntelliJ IDEA.
- Git.

### 2. Clone o repositório

```bash
git clone https://github.com/SEU-USUARIO/Pet-mania-API.git
```

Entre na pasta do projeto:

```bash
cd Pet-mania-API
```

### 3. Configure o banco de dados

Crie o banco de dados no MySQL:

```sql
CREATE DATABASE Pet_Mania;
```

Configure o arquivo `application.properties` com as credenciais do seu MySQL:

```properties
spring.application.name=petMania

spring.datasource.url=jdbc:mysql://localhost:3306/Pet_Mania
spring.datasource.username=SEU_USUARIO
spring.datasource.password=SUA_SENHA

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
```

### 4. Execute a aplicação

Abra o projeto na sua IDE e execute a classe:

`PetManiaApplication.java`

A API estará disponível em:

```http
http://localhost:8080
```

O Front-end poderá ser acessado pelo mesmo endereço, pois está localizado na pasta `static` do projeto.

## 🧪 Testes com Postman

Os endpoints foram testados utilizando o Postman, verificando as operações de consulta, cadastro, atualização e exclusão de animais.

### Evidências dos testes

**GET — Listar animais**

<img width="900" alt="image" src="https://github.com/user-attachments/assets/faa1236c-a61d-473f-b59e-b4d8276f4e67" />

## 🖥️ Demonstração do Front-end

O projeto também conta com uma interface para facilitar o gerenciamento dos animais.

### Tela inicial

<img width="900"  alt="image" src="https://github.com/user-attachments/assets/0db32a09-20ec-404c-bf91-a65608744340" />


### Cadastro de animal

<img width="900" alt="image" src="https://github.com/user-attachments/assets/7ae91735-63c0-4380-b5fc-e053852aa4f1" />

### Atualização de animal

<img width="900"  alt="image" src="https://github.com/user-attachments/assets/5f749078-cb07-462a-8374-4c9427fdf17a" />

## 📚 Aprendizados

Durante o desenvolvimento deste desafio, foi possível praticar:

- Análise e correção de erros em projetos Java.
- Desenvolvimento de APIs REST com Spring Boot.
- Integração entre Java e MySQL.
- Utilização do Spring Data JPA.
- Implementação de operações CRUD.
- Testes de requisições HTTP com Postman.
- Integração entre Back-end e Front-end.
- Versionamento de código com Git e GitHub.

## 👨‍💻 Autor

Desenvolvido por **Felipe Lisboa Carvalho**.

Projeto acadêmico realizado como parte do desafio Pet Mania.
