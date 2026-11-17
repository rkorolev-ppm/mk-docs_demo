# Работа с документацией

## Локальный запуск

```bash
git clone https://github.com/rkorolev-ppm/mk-docs_demo.git
cd mk-docs_demo
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.lock
mkdocs serve
```

Откройте http://127.0.0.1:8000. Правьте Markdown в `docs/` — страница обновится.

## Pull Request

1. Создайте ветку: `git switch -c docs/change-guide`.
2. Измените документ и выполните `mkdocs build --strict`.
3. Сохраните изменения коммитом и отправьте ветку.
4. Откройте PR в `main`, дождитесь проверки и ревью.

## Сборка

CI проверяет PR и основную ветку, сохраняет готовый сайт как артефакт.
Каталог `site/` можно обслуживать любым статическим веб-сервером.
Приватность репозитория сама по себе не обеспечивает приватность размещённого сайта.
