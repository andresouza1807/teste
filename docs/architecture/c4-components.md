# C4 - Componentes

Detalhamento interno do orquestrador.

```mermaid
flowchart TB
    Orchestrator[Orquestrador]

    Orchestrator --> Scheduler[Scheduler]
    Orchestrator --> TaskRouter[Task Router]
    Orchestrator --> RetryManager[Retry Manager]
    Orchestrator --> StateManager[State Manager]
    Orchestrator --> AuditTrail[Audit Trail]
    Orchestrator --> PolicyEngine[Policy Engine]

    TaskRouter --> Broker[(Message Broker)]
    StateManager --> DB[(PostgreSQL)]
    AuditTrail --> Logs[(Logs Storage)]
```

## Componentes
- **Scheduler:** agenda jobs
- **Task Router:** distribui tarefas para workers
- **Retry Manager:** aplica backoff e retentativas
- **State Manager:** controla estados
- **Audit Trail:** garante rastreabilidade
- **Policy Engine:** regras e limites operacionais
