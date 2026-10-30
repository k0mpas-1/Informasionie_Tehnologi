# Портлингва — сайт и сквозная аналитика заявок

Практическая работа по дисциплине ОП.03 «Информационные технологии», ТЗ № ТЗ-05/2026, АНО ДО «Портлингва». Исполнитель: Михеев Николай Сергеевич, группа РПО-26/1/11.

Сайт школы иностранных языков: каждый посетитель приходит с меткой источника, каждая заявка попадает в Google Таблицу, а по данным GA4 видно, какой канал приводит клиентов.

![Схема работы](docs/scheme.png)

## Ссылки

| Что | Ссылка |
|---|---|
| Сайт | https://portlingva.vercel.app |
| Репозиторий | https://github.com/k0mpas-1/portlingva |
| Описание работы | [docs/opisanie.md](docs/opisanie.md) |
| Реестр UTM-ссылок | [docs/utm-registry.md](docs/utm-registry.md) |
| События GA4 | [docs/events.md](docs/events.md) |
| Запросы к ИИ | [docs/prompts.md](docs/prompts.md) |
| Презентация к защите | [presentation/zashchita.pdf](presentation/zashchita.pdf) |

Measurement ID ресурса GA4: `G-2CZ494QV10`.

## Что сделано

| Часть | Результат |
|---|---|
| Сайт | 10 страниц, статический HTML/CSS/JS, опубликован на Vercel |
| GA4 | ресурс создан, Measurement ID `G-2CZ494QV10`, события отправляются из `js/analytics.js` |
| UTM | реестр из 7 ссылок с метками source, medium и campaign |
| Заявки | форма → Google Apps Script → лист `leads`, проверка полей и повторов по `request_id` |
| Instagram | автоответы ManyChat на комментарий под Reel с кнопкой на сайт в Direct |
| Отчёты | Reports и Explore в GA4, воронка заявки |

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

HTML, CSS, JavaScript · Google Analytics 4 · Google Таблицы и Apps Script · ManyChat · GitHub и Vercel. Сайт создан с помощью claude и доработан вручную, документация оформлена с частичной помощью claude

## Структура

```
index.html …         страницы сайта
js/analytics.js      события GA4
js/form.js           отправка формы
apps-script/Code.gs  приёмник заявок
docs/                описание, реестр UTM, события, запросы к ИИ, схема
screens/             скриншоты по разделам ТЗ
presentation/        презентация к защите
```
