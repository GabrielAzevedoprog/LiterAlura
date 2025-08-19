# 📚 Literalura

<div align="center">
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT" />
  </a>
  <img src="https://img.shields.io/badge/Java-8%2B-blue" alt="Java Version" />
</div>

---

Projeto desenvolvido durante o programa **ONE - Oracle Next Education**, em parceria com a **Alura** e a **Oracle**.

Literalura é uma aplicação Java com Spring Boot que consome a API do Projeto Gutenberg para registrar, consultar e organizar livros e autores.

---

## 🏅 Badge

<div align="center">
  <img src="img/badge%20literalura.png" alt="Badge do Projeto Literalura" />
</div>

---

## 🚀 Instalação

Siga os passos abaixo para rodar o projeto localmente:

### 1. Clone o repositório

### 2. Configure o banco de dados

Edite o arquivo `src/main/resources/application.properties` com as informações do seu PostgreSQL:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/literalura
spring.datasource.username=seu-usuario
spring.datasource.password=sua-senha
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

> 💡 Certifique-se de que o PostgreSQL esteja rodando e que o banco `literalura` já exista.

### 3. Execute a aplicação

```bash
mvn spring-boot:run
```

---

## 🧠 Estrutura do Projeto

```
br.com.alura.literalura
├── principal          # Classe Principal que inicia a aplicação
├── model              # Entidades: Livro, Autor, DTOs
├── repository         # Interfaces JPA (LivroRepository, AutorRepository)
├── service            # Lógicas de negócio e consumo de API
```

---

## 📌 Funcionalidades

* 📥 Consumo da API do Projeto Gutenberg
* 📚 Registro e persistência de livros e autores
* 🔍 Filtros por autor, idioma, ano de publicação, entre outros
* 🗃️ Integração com banco de dados PostgreSQL

---

## 🤝 Contribuindo

Contribuições são sempre bem-vindas!
Você pode:

* Reportar bugs
* Sugerir melhorias
* Criar pull requests com novas funcionalidades

---

## 📄 Licença

Este projeto está sob a licença [MIT](LICENSE).
