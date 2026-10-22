# pravoresheniya.ru

Статический сайт юридической компании «Правовые решения». Размещается на GitHub Pages из ветки `main`, корень репозитория.

- `index.html` — вся страница, стили внутри.
- `fonts/`, `fonts.css` — Cormorant Garamond и Golos Text (latin + cyrillic), самохост.
- `img/` — фотографии.
- Свой домен пока не подключён: сайт живёт на https://neurolegal.github.io/pravoresheniya-site/. Для pravoresheniya.ru добавить файл `CNAME` с доменом и DNS-записи ниже.

Форма заявки пока не отправляет данные: нужен бэкенд (Telegram-бот или почта).

## DNS (один раз, у регистратора или в Tilda DNS)

| Имя | Тип | Значение |
|---|---|---|
| @ (pravoresheniya.ru) | A | 185.199.108.153 |
| @ | A | 185.199.109.153 |
| @ | A | 185.199.110.153 |
| @ | A | 185.199.111.153 |
| www | CNAME | neurolegal.github.io |

Старые записи Tilda (A 176.57.65.30) удалить. После того как DNS обновится, в настройках репозитория Settings → Pages включить «Enforce HTTPS» (сертификат GitHub выпускает сам, обычно до часа).

## Как обновлять

Править `index.html` и пушить в `main` — GitHub Pages пересобирает сайт за минуту.
