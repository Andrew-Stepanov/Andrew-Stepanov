# Безопасность

## Расписание

Раз в неделю агент проверяет активные репозитории на:

- `npm audit` (critical/high в приоритете)
- секреты в исходниках
- статус Dependabot / workflows
- грубые проблемы гигиены (закоммиченный `node_modules`, открытые эндпоинты)

Отчёты: [`.security/reports/`](../.security/reports/).

## Как запускать

1. Cursor Automation с промптом из [`.security/WEEKLY_PROMPT.md`](../.security/WEEKLY_PROMPT.md).
2. Или ручной запуск Cloud Agent с тем же текстом.

## Приоритеты фикса

1. `frontier` — обновить Next.js (≥16.3.6).
2. `popup` / `webhook-progkids` — `npm audit fix`, major-обновления sendgrid/sqlite3/axios.
3. Включить Dependabot alerts на GitHub.
