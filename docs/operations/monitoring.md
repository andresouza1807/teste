# Monitoramento

## Objetivo
Garantir visibilidade de performance e falhas.

## Métricas recomendadas
### Orquestrador
- jobs/min
- tempo médio execução
- taxa de erro
- backlog da fila

### Workers
- workers online/offline
- consumo CPU/RAM
- falhas por tipo

### Banco
- conexões
- slow queries
- locks

## Ferramentas
- Prometheus + Grafana
- Loki / ELK
- Jaeger
