**12. Esquema de Base de Dados**

USER

| Campo      | Tipo    |
| ---------- | ------- |
| user_id    | UUID    |
| nome       | VARCHAR |
| email      | VARCHAR |
| unidade_id | UUID    |


UNIT

| Campo   | Tipo    |
| ------- | ------- |
| unit_id | UUID    |
| bloco   | VARCHAR |
| numero  | VARCHAR |


CHARGER

| Campo      | Tipo    |
| ---------- | ------- |
| charger_id | UUID    |
| serial     | VARCHAR |
| modelo     | VARCHAR |


SESSION

| Campo       | Tipo      |
| ----------- | --------- |
| session_id  | UUID      |
| user_id     | UUID      |
| charger_id  | UUID      |
| inicio      | TIMESTAMP |
| fim         | TIMESTAMP |
| energia_kwh | DECIMAL   |

INVOICE

| Campo       | Tipo    |
| ----------- | ------- |
| invoice_id  | UUID    |
| user_id     | UUID    |
| referencia  | DATE    |
| valor_total | DECIMAL |


**13. Registros Simulados**

```json
{
  "user_id":"U001",
  "nome":"Carlos Silva",
  "unidade":"A-203"
}
```
```json
{
  "session_id":"S0001",
  "user_id":"U001",
  "charger_id":"GW001",
  "energy_kwh":22.4,
  "duration":190
}
```
```json
{
  "invoice_id":"F0001",
  "user_id":"U001",
  "month":"2026-06",
  "energy_kwh":85.6,
  "value":93.18
}
```
