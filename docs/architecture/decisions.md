# ADR - Architecture Decision Records

Registro de decisões técnicas importantes.

---

## ADR-001 - Uso de Message Broker

**Status:** Aprovado  
**Data:** 2026-02-12  

### Contexto
Precisamos desacoplar o orquestrador dos workers e suportar execução distribuída.

### Decisão
Utilizar RabbitMQ (ou Kafka) como mecanismo central de filas/eventos.

### Consequências
- Escalabilidade horizontal
- Retentativas e reprocessamento
- Maior complexidade operacional
