# Тестовый MkDocs

Демонстрационные данные; внутренних документов нет.

Локальный запуск:

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.lock
mkdocs serve
```

Проверка: `mkdocs build --strict`. Готовый сайт — `site/`.
CI собирает сайт для PR и main и сохраняет артефакт на 7 дней.
Размещение GitHub Pages для приватного репозитория зависит от тарифа;
workflow не публикует сайт автоматически.

Используются MkDocs 1.6.1 и Material 9.7.0. Material завершает поддержку
5 мая 2027 года: для постоянной корпоративной установки тему следует выбрать отдельно.
