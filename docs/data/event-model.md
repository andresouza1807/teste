# Modelo de Eventos

Este documento descreve os eventos publicados no broker.

## Exemplo de evento
```json
{
  "event_id": "evt_123",
  "job_id": "job_999",
  "type": "SEND_MESSAGE",
  "created_at": "2026-02-12T20:00:00Z",
  "payload": {
    "target": "whatsapp",
    "message": "Olá!"
  }
}
```
