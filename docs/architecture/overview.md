# Visão Geral da Arquitetura

Este documento descreve a arquitetura macro da plataforma.

## Visão geral
A plataforma recebe demandas (jobs), executa decisão via agentes IA e delega a execução para workers.

### Componentes principais
- UI/Dashboard
- Orquestrador
- Core de agentes IA
- Broker (RabbitMQ/Kafka)
- Workers RPA
- Banco PostgreSQL
- Cache Redis
- Observabilidade (logs/métricas/traces)
