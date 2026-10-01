# Промпт для Cursor Automation (раз в неделю)

```
Проведи еженедельную проверку уязвимостей по активным репозиториям Andrew-Stepanov
(frontier, webhook-progkids, popup и другим с package.json):

1. Склонируй/проверь репозитории, запусти npm audit.
2. Просканируй исходники на секреты и .env.
3. Отметь Dependabot / code scanning статус.
4. Сохрани отчёт в .security/reports/YYYY-MM-DD.md в репозитории профиля.
5. Создай черновик письма на andrewa.stepanov@gmail.com с краткой сводкой
   (critical/high и конкретные действия).
6. Открой PR только если меняется отчёт или конфигурация безопасности.
Не правь production-код без явного запроса — сначала отчёт.
```
