## Gabriel Ferreira

**Backend engineer** — Java 21 · Kotlin · Spring Boot

Trabalho na OTI Software no **SIGESCANTT**, sistema de gestão para uma agência
reguladora federal (ANTT). É um Maven multi-módulo — server, services, shared,
schedulers, GED e dois SDKs de integração — rodando Spring Boot com Keycloak,
PostgreSQL e SQL Server na mesma aplicação, Liquibase para versionar schema,
Spring Batch e Quartz para as rotinas noturnas, e Testcontainers na suíte.

É o tipo de sistema onde a decisão errada não aparece no dia do deploy: aparece
seis meses depois, num job que roda às 3h e ninguém está olhando. Foi ali que
aprendi a me importar com idempotência, com o que acontece quando o terceiro
está fora do ar, e com deixar o rastro que o próximo dev vai precisar ler.

### No que estou focado

- **Jobs em lote que sobrevivem a arquivo sujo** — chunk, skip policy, restart
- **Processamento assíncrono** — desacoplar o que é lento do ciclo request/response
- **Fronteira de módulo** — onde separar, o que expor, o que manter privado

### Projetos

**[batchaurant](https://github.com/gabrielbkx/batchaurant)** — Importação de pedidos por CSV com Spring Batch.
Arquivo de verdade vem sujo: data em formato errado, mesa que não é número,
valor negativo. A pergunta que o projeto responde é quando uma linha ruim deve
derrubar o lote e quando deve ser só posta de lado. Tem `SkipPolicy` própria
classificando o tipo de falha, chunks de 100, e um Step de validação que **para
o job de propósito** para você confirmar antes de gravar.
`Java 21 · Spring Boot · Spring Batch · PostgreSQL · 48 testes`

**[FestConnect](https://github.com/gabrielbkx/FestConnect)** — API de marketplace ligando organizadores de eventos a prestadores.
Catálogo modelado com herança JOINED (`Produto`, `Servico` e `Local` estendendo
`ItemCatalogo`), busca por raio com Haversine, upload em S3 com thumbnail, e
rastreamento distribuído com OpenTelemetry + Jaeger.
`Java 21 · Spring Boot · PostgreSQL · Security + OAuth2 · S3 · OpenTelemetry`

**[nutau](https://github.com/gabrielbkx/nutau)** — Banco digital com solicitação de crédito.
A análise consulta dois bureaus externos e leva segundos. Segurar a conexão HTTP
esperando custaria uma thread por cliente e amarraria a disponibilidade da minha
API à de um terceiro — então o endpoint aceita, responde **202** e devolve o id
para acompanhamento. A mensageria que vai consumir esse fluxo é a Fase 2, e o
ponto exato do corte está marcado no código.
`Java 21 · Spring Boot 3 · PostgreSQL · Liquibase · JWT · MapStruct`

---

[LinkedIn](https://www.linkedin.com/in/gabrielolif) · [Portfólio](https://gabrielolif.vercel.app) · oliveiraferreira97@gmail.com
