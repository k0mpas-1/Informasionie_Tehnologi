[README.md](https://github.com/user-attachments/files/34157466/README.md)
# Портлингва — сайт и сквозная аналитика заявок

Практическая работа по дисциплине ОП.03 «Информационные технологии», ТЗ № ТЗ-05/2026, АНО ДО «Портлингва». Исполнитель: Михеев Николай Сергеевич, группа РПО-26/1/11.

Сайт школы иностранных языков: каждый посетитель приходит с меткой источника, каждая заявка попадает в Google Таблицу, а руководитель видит на дашборде, какой канал приводит клиентов.

![Схема работы](docs/scheme.png)

## Ссылки

| Что | Ссылка |
|---|---|
| Сайт | https://portlingva.vercel.app |
| Репозиторий | https://github.com/k0mpas-1/portlingva |
| Таблица заявок | ___ |
| Дашборд DataLens | ___ |
| Instagram и Reel с автоответом | ___ |
| ВКонтакте · Telegram · YouTube | ___ · ___ · ___ |
| Описание работы | [docs/opisanie.md](docs/opisanie.md) |
| Реестр UTM-ссылок | [docs/utm-registry.md](docs/utm-registry.md) |
| События GA4 | [docs/events.md](docs/events.md) |
| Презентация к защите | [presentation/zashchita.pdf](presentation/zashchita.pdf) |

Ресурс GA4: `G-___`. Доступ Viewer к ресурсу GA4 выдан: ___ (e-mail преподавателя).

## Что сделано

| Часть | Результат |
|---|---|
| Сайт | 10 страниц, статический HTML/CSS/JS, Vercel, Lighthouse: ___ / ___ / ___ |
| GA4 | ___ событий, ___ пользовательских параметров, ключевое: `generate_lead` |
| UTM | ___ ссылок в реестре, публикации в ___ соцсетях |
| Заявки | форма → Apps Script → лист `leads`, проверка полей и повторов по `request_id` |
| Instagram | ManyChat, две ветки: `___` и `___` |
| Отчёты | Reports, Explore, воронка, дашборд DataLens |

## Страницы сайта

- `index.html` — главная
- `courses.html` — курсы
- `level-test.html` — тест уровня из 12 вопросов
- `teachers.html` — преподаватели
- `prices.html` — цены
- `phrases.html` — 50 фраз и промокод
- `contacts.html` — форма заявки
- `thanks.html` — подтверждение
- `privacy.html` — политика конфиденциальности
- `404.html` — страница ошибки

## Технологии

HTML, CSS, JavaScript · Google Analytics 4 · Google Таблицы и Apps Script · ManyChat · Yandex DataLens · GitHub и Vercel. Сайт создан с помощью ChatGPT (запросы — в [docs/prompts.md](docs/prompts.md)) и доработан вручную.

## Структура

```
index.html …         страницы сайта
js/analytics.js      все события GA4
js/form.js           отправка формы
apps-script/Code.gs  приёмник заявок
docs/                описание, реестр UTM, события, запросы к ИИ, схема
screens/             кадры-доказательства по разделам ТЗ
presentation/        презентация к защите
```

## Итог

Не получилось: -

Нейросеть использовалась для: подготовки стартовой структуры сайта, текстов, HTML/CSS/JS и документации , оформления описания работы
