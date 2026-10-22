# Node.js CI Practice

Мінімальний Node.js-проєкт для практичної роботи з GitHub Actions.

## Запуск локально

Потрібен Node.js 22 або сумісна актуальна версія.

```bash
npm install
npm run build
npm start
```

Очікуваний вивід:

```text
Hello world
```

## GitHub Actions

Workflow розташований у `.github/workflows/ci.yml` і запускається при кожному `push` до гілки `main`.

Він:
1. Завантажує код репозиторію.
2. Встановлює Node.js 22.
3. Виконує `npm install`.
4. Виконує `npm run build`.
5. Зберігає файли проєкту як артефакт `nodejs-build`.

Після завантаження проєкту в публічний GitHub-репозиторій відкрий вкладку **Actions** і перевір результат запуску.
