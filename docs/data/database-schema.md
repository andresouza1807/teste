# Banco de Dados (PostgreSQL)

## Objetivo
Persistir:
- jobs
- execuções
- auditoria
- estado de workers

## Tabelas sugeridas
### jobs
- id
- type
- payload
- status
- created_at

### executions
- id
- job_id
- worker_id
- started_at
- finished_at
- status
- error_message

### audit_log
- id
- job_id
- action
- result
- created_at
