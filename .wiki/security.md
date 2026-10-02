# Безопасность

## Расписание

Раз в неделю агент проверяет репозитории (кроме исключений) на:

- `npm audit` (critical/high в приоритете)
- секреты в исходниках
- статус Dependabot / workflows
- грубые проблемы гигиены (закоммиченный `node_modules`, открытые эндпоинты)

Отчёты: [`.security/reports/`](../.security/reports/).

## Исключения

Не проверять (заброшены, 2026-10-02): `frontier`, `webhook-progkids`, `popup`.  
Список: [`.security/SKIP.md`](../.security/SKIP.md).

## Как запускать

1. Cursor Automation с промптом из [`.security/WEEKLY_PROMPT.md`](../.security/WEEKLY_PROMPT.md).
2. Или ручной запуск Cloud Agent с тем же текстом.
