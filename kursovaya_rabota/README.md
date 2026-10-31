# Курсовая работа · «Портлингва»

**Сайт языковой школы и сквозная аналитика заявок**
ОП.03 «Информационные технологии» · ТЗ № ТЗ-05/2026 · АНО ДО «Портлингва»
Михеев Николай Сергеевич, группа РПО-26/1/11

![Схема работы](docs/scheme.png)

## Ссылки

| Что | Где |
|---|---|
| Сайт | https://portlingva.vercel.app |
| Репозиторий проекта | https://github.com/k0mpas-1/portlingva |
| Таблица заявок «Portlingva — Leads» | https://docs.google.com/spreadsheets/d/1B8_DCw0lP4tSj5M1etOccMogSZzZ1N2-YNo8vCztiaw/edit |
| Instagram | https://www.instagram.com/k0mpas_1/ |
| Презентация к защите (14 слайдов) | [presentation/zashchita.pdf](presentation/zashchita.pdf) |
| Описание работы | [docs/opisanie.md](docs/opisanie.md) |
| Бланк сдачи | [kursovaya.md](kursovaya.md) |

GA4: ресурс «Портлингва», Measurement ID `G-2CZ494QV10`.

## Состав папки

```
kursovaya_rabota/
├── README.md             этот файл
├── kursovaya.md          бланк сдачи с чек-листом
├── docs/
│   ├── opisanie.md       описание работы по разделам ТЗ
│   ├── events.md         20 событий GA4 с файлом и строкой
│   ├── utm-registry.md   реестр 12 UTM-ссылок
│   ├── prompts.md        журнал запросов к нейросети
│   └── scheme.png        схема работы
└── presentation/
    └── zashchita.pdf     презентация к защите
```

Код сайта, приёмник заявок, инструкции и скриншоты — в репозитории проекта [k0mpas-1/portlingva](https://github.com/k0mpas-1/portlingva).

## Статус по разделам ТЗ

| Раздел | Статус | Результат |
|---|---|---|
| 3. Сайт | ✅ | 10 страниц на Vercel, адаптив 375 / 768 / 1280, Lighthouse mobile 99 / 94 / 100 / 100 |
| 4. GA4 | ✅ | 20 событий из `js/analytics.js`, 7 пользовательских параметров, 3 ключевых события, правило `lang_to_language` |
| 5. UTM | ✅ | 12 ссылок, QR-код U-12, афиша A4 |
| 6. Заявки | ✅ | форма → Apps Script → лист `leads`, проверка, защита от дублей, статусы до оплаты |
| 7. Instagram | ✅ | бизнес-аккаунт, Reel «5 фраз», ManyChat Live: ветки ФРАЗЫ (U-02) и КИТАЙСКИЙ (U-03) |
| 8. Отчёты GA4 | ✅ | свободная форма, воронка (4 вкладки), путь, обратный путь, атрибуция, оповещение |
| 8.4. DataLens | ❌ | сервис не работал; описание дашборда — [docs/datalens.md](https://github.com/k0mpas-1/portlingva/blob/main/docs/datalens.md) |
| Публикации VK, Telegram, YouTube | ❌ | не публиковались; ссылки U-05…U-09 готовы в реестре |
| Живой тест ManyChat | ⚠️ | нет второго аккаунта Instagram; сценарии проверены в предпросмотре |
| 11. Документация | ✅ | README проекта, описание, события, UTM, запросы к ИИ, презентация |

## Что осталось сделать перед сдачей

- [ ] Добавить ссылку U-01 в профиль Instagram (с телефона: «Редактировать профиль» → «Ссылки»):
  `https://portlingva.vercel.app/?utm_source=instagram&utm_medium=social&utm_campaign=trial_jan_2027&utm_content=bio`
- [ ] Выдать преподавателю доступ Viewer к ресурсу GA4 и доступ на просмотр к таблице
- [ ] Сделать репозиторий `portlingva` публичным, заполнить описание, Website и Topics
- [ ] Прогнать доклад по презентации — уложиться в 7 минут

## Нейросеть

Claude — подсказки по коду, текстам и документации. Запросы — в [docs/prompts.md](docs/prompts.md).
