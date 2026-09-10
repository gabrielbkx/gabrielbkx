<div align="center">

# Gabriel Ferreira

### ☕ Backend Engineer · Java · Kotlin · Spring Boot

<p>
  <a href="https://www.linkedin.com/in/gabrielolif">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="https://gabrielolif.vercel.app">
    <img src="https://img.shields.io/badge/Portfólio-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfólio" />
  </a>
  <a href="mailto:oliveiraferreira97@gmail.com">
    <img src="https://img.shields.io/badge/E--mail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="E-mail" />
  </a>
  <a href="https://wa.me/5522998715889">
    <img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp" />
  </a>
</p>

</div>

---

## 🏢 No que eu trabalho

Desenvolvo o **SIGESCANTT** na **OTI Software** — sistema de gestão para uma agência
reguladora federal (**ANTT**). É um Maven multi-módulo com *server*, *services*, *shared*,
*schedulers*, GED e dois SDKs de integração, rodando Spring Boot com Keycloak,
**PostgreSQL e SQL Server na mesma aplicação**, Liquibase versionando schema e
Spring Batch + Quartz nas rotinas noturnas.

> É o tipo de sistema onde a decisão errada não aparece no deploy — aparece seis meses
> depois, num job que roda às 3h e ninguém está olhando. Foi ali que aprendi a me importar
> com idempotência, com o que acontece quando o terceiro cai, e com deixar o rastro que o
> próximo dev vai precisar ler.

---

## 🛠️ Stack

#### ☕ Linguagens
![Java](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

#### 🍃 Framework
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![Spring Batch](https://img.shields.io/badge/Spring_Batch-6DB33F?style=flat-square&logo=spring&logoColor=white)
![WebFlux](https://img.shields.io/badge/WebFlux-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Quartz](https://img.shields.io/badge/Quartz-1E88E5?style=flat-square&logo=clockify&logoColor=white)

#### 🗄️ Persistência
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=flat-square&logo=hibernate&logoColor=white)
![Liquibase](https://img.shields.io/badge/Liquibase-2962FF?style=flat-square&logo=liquibase&logoColor=white)

#### 📨 Mensageria & Infra
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=flat-square&logo=keycloak&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)

#### 🧪 Qualidade
![JUnit5](https://img.shields.io/badge/JUnit_5-25A162?style=flat-square&logo=junit5&logoColor=white)
![Testcontainers](https://img.shields.io/badge/Testcontainers-291A3F?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=opentelemetry&logoColor=white)

---

## 🚀 Projetos

### 🍽️ [batchaurant](https://github.com/gabrielbkx/batchaurant) — importação em lote que aguenta arquivo sujo

Arquivo de verdade vem com data em formato errado, mesa que não é número, valor negativo.
A pergunta que o projeto responde: **quando uma linha ruim deve derrubar o lote e quando
deve ser só posta de lado?** Tem `SkipPolicy` própria classificando o tipo de falha, chunks
de 100 e um Step de validação que **para o job de propósito** para você confirmar antes de gravar.

![Java](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Batch](https://img.shields.io/badge/Spring_Batch-6DB33F?style=flat-square&logo=spring&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![48 testes](https://img.shields.io/badge/48_testes-25A162?style=flat-square&logo=junit5&logoColor=white)

### 🎉 [FestConnect](https://github.com/gabrielbkx/FestConnect) — marketplace de eventos

Conecta organizadores a prestadores. Catálogo modelado com **herança JOINED** (`Produto`,
`Servico` e `Local` estendendo `ItemCatalogo`), busca por raio com Haversine, upload em S3
com geração de thumbnail e rastreamento distribuído com OpenTelemetry + Jaeger.

![Java](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![OAuth2](https://img.shields.io/badge/OAuth2-EB5424?style=flat-square&logo=auth0&logoColor=white)
![AWS S3](https://img.shields.io/badge/AWS_S3-569A31?style=flat-square&logo=amazons3&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=opentelemetry&logoColor=white)

### 🏦 [nutau](https://github.com/gabrielbkx/nutau) — banco digital com crédito assíncrono

A análise consulta dois bureaus externos e leva segundos. Segurar a conexão HTTP esperando
custaria **uma thread por cliente** e amarraria a disponibilidade da minha API à de um
terceiro — então o endpoint aceita, responde **`202 Accepted`** e devolve o id para
acompanhamento. A mensageria que vai consumir esse fluxo é a Fase 2, com o ponto de corte
marcado no código.

![Java](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![Liquibase](https://img.shields.io/badge/Liquibase-2962FF?style=flat-square&logo=liquibase&logoColor=white)

### 📮 [cep-service](https://github.com/gabrielbkx/cep-service) — API de CEP com pipeline completo

Autenticação JWT, cache e **CI/CD no GitHub Actions com deploy ativo no Render**.
Desafio técnico levado até o fim: build, testes e entrega automatizados.

![Java](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI%2FCD-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Render](https://img.shields.io/badge/Deploy-46E3B7?style=flat-square&logo=render&logoColor=white)

---

## 🎯 No que estou focado agora

- 📨 **Processamento assíncrono** — desacoplar o que é lento do ciclo request/response
- 🔁 **Jobs em lote resilientes** — chunk, skip policy, restart e idempotência
- 🧩 **Fronteira de módulo** — onde separar, o que expor, o que manter privado

---

<div align="center">

### 📊 GitHub

<img width="88%" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=gabrielbkx&theme=tokyonight" alt="Resumo do perfil" />

<img height="200" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=gabrielbkx&theme=tokyonight" alt="Linguagens por commit" />
<img height="200" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=gabrielbkx&theme=tokyonight" alt="Linguagens por repositório" />

<br><br>

💬 Aberto a oportunidades **backend** — Java · Kotlin · Spring Boot

</div>
