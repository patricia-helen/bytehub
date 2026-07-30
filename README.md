# ByteHUB

Sistema open source de gestão de liga acadêmica, desenvolvido com base em requisitos levantados junto à Liga Acadêmica ByteBuilders da UFVJM. Gerencia membros, grupos (guildas e projetos), encontros, presenças e histórico de gestões.

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)
![Java](https://img.shields.io/badge/Java-21-orange)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-4.1.0-brightgreen)

## 📋 Sobre o projeto

O ByteHUB nasceu da necessidade real da Liga Acadêmica ByteBuilders de organizar seus processos internos: cadastro de membros, formação de guildas e grupos de projeto, registro de encontros e controle de presença (com regra de frequência mínima para certificação). O projeto também serve como portfólio técnico, aplicando boas práticas de arquitetura back-end Java.

## 🚀 Tecnologias

| Categoria | Stack |
|---|---|
| Linguagem | Java 21 |
| Framework | Spring Boot 4.1.0 |
| Segurança | Spring Security + JWT |
| Persistência | Spring Data JPA + PostgreSQL |
| Containerização | Docker + Docker Compose |
| Documentação de API | Springdoc / Swagger |
| Build | Maven |

## 📦 Estrutura do projeto

``
com.patriciahelen.bytehub
- config      → configurações gerais do Spring (segurança, beans)
- security    → autenticação JWT, filtros, UserDetailsService
```

*(estrutura em expansão conforme novas sprints avançam)*

## ⚙️ Como rodar localmente

**Pré-requisitos:** Java 21, Docker e Docker Compose instalados.

```bash
# 1. Clonar o repositório
git clone https://github.com/patricia-helen/bytehub.git
cd bytehub

# 2. Subir o banco de dados PostgreSQL
docker compose up -d

# 3. Rodar a aplicação
./mvnw spring-boot:run
```

A aplicação sobe por padrão em `http://localhost:8080`.

## 🗺️ Roadmap (Sprints)

| Sprint | Entrega | Foco técnico |
|---|---|---|
| 1 | Setup + Auth | Spring Boot init, PostgreSQL, Docker, Spring Security + JWT |
| 2 | *(em planejamento)* | — |

## 📄 Licença

Este projeto está licenciado sob a licença MIT — veja o arquivo [LICENSE](LICENSE) para mais detalhes.
