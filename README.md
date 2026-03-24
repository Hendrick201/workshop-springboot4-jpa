# 🛒 API REST - Gerenciamento de Pedidos

API RESTful para gerenciamento de pedidos desenvolvida com **Java + Spring Boot**, aplicando boas práticas de arquitetura em camadas, persistência com JPA/Hibernate e banco de dados H2 em memória para ambiente de desenvolvimento.

---

## 🚀 Tecnologias Utilizadas

| Tecnologia | Versão |
|---|---|
| Java | 25 |
| Spring Boot | 4.0.3 |
| Spring Data JPA | - |
| Hibernate / Jakarta EE | - |
| H2 Database (dev) | - |
| PostgreSQL (prod) | - |
| Maven | - |

---

## 📐 Arquitetura

O projeto segue o padrão de **Arquitetura em Camadas**:

```
src/
└── main/
    └── java/
        └── com.educandoweb.course/
            ├── controllers/   # Endpoints REST
            ├── services/      # Regras de negócio
            ├── repositories/  # Acesso a dados (JPA)
            └── entities/      # Modelos de domínio
```

---

## ⚙️ Funcionalidades

- ✅ CRUD completo de pedidos
- ✅ Relacionamento entre entidades (Pedido, Produto, Usuário, etc.)
- ✅ Persistência com JPA/Hibernate
- ✅ Banco H2 em memória para desenvolvimento e testes
- ✅ Suporte a PostgreSQL para ambiente de produção

---

## 🗄️ Console H2

Durante o desenvolvimento, o banco de dados H2 pode ser acessado pelo console web:

```
URL: http://localhost:8080/h2-console
JDBC URL: jdbc:h2:mem:testdb
User: sa
Password: (vazio)
```

---

## ▶️ Como Executar

### Pré-requisitos
- Java 25+
- Maven

### Passos

```bash
# Clone o repositório
git clone https://github.com/Hendrick201/API-REST-de-Gerenciamento-de-Pedidos-com-Spring-Boot.git

# Entre na pasta do projeto
cd API-REST-de-Gerenciamento-de-Pedidos-com-Spring-Boot

# Execute com Maven
./mvnw spring-boot:run
```

A API estará disponível em: `http://localhost:8080`

---

## 📡 Endpoints

| Método | Rota | Descrição |
|---|---|---|
| GET | `/orders` | Lista todos os pedidos |
| GET | `/orders/{id}` | Busca pedido por ID |
| POST | `/orders` | Cria novo pedido |
| PUT | `/orders/{id}` | Atualiza pedido |
| DELETE | `/orders/{id}` | Remove pedido |

> Os endpoints de outras entidades (usuários, produtos) seguem o mesmo padrão.

---

## 👨‍💻 Autor

**Hendrick Miqueias De Oliveira Gomes**  
Estudante de ADS – IFTM | Backend Java Developer  

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/Hendrick-Miqueias)

