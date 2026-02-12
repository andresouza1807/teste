# Runbook - Fila Travada

## Sintomas
- backlog crescente
- mensagens não sendo consumidas
- worker ativo mas sem processamento

## Ações
1. Verificar broker
2. Verificar workers online
3. Checar dead-letter queue
4. Reiniciar consumidores se necessário
