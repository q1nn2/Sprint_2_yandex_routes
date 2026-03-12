# Яндекс Маршруты — Итоговый проект 2 спринта

Репозиторий с результатами ручного тестирования веб‑сервиса **Яндекс Маршруты**: тест-анализ, классы эквивалентности и граничные значения, тест-кейсы, баг-репорты.

## Ссылки

- Сервис: https://qa-routes.praktikum-services.ru/
- Требования: https://docs.google.com/document/d/1tIs3KqK79vGR60EoGiDKLavvgsj0cjjrdSRK3AFdY6g/edit
- Рабочая таблица (Google Sheets): https://docs.google.com/spreadsheets/d/1ku3De2DZUbj_QlJKdQU7wEh0N3EIILJ8D6_vwkshmQU/edit

## Артефакты

- ✅ **Тест-анализ**
  - 📄 [`analysis/overview.md`](analysis/overview.md)
  - Вкладка Google Sheets: «Этап 1. Тест-анализ»

- ✅ **КЭ и ГЗ**
  - 📄 [`ce-gz/time-fields.md`](ce-gz/time-fields.md)
  - 📄 [`ce-gz/address-fields.md`](ce-gz/address-fields.md)
  - 📄 [`ce-gz/routes-and-time-intervals.md`](ce-gz/routes-and-time-intervals.md)
  - Вкладка Google Sheets: «Этап 2. КЭ и ГЗ»

- ✅ **Тест-кейсы**
  - 📁 [`testcases/`](testcases)
  - Вкладка Google Sheets: «Этап 3. Тест-кейсы»
  - Примеры групп:
    - `TC-hours.md` — валидация поля **Часы** (`T1–T24`)
    - `TC-minutes.md` — валидация поля **Минуты** (`T25–T48`)
    - `TC-from-address.md` — поле **Откуда** (`T49–T53`)
    - `TC-to-address.md` — поле **Куда** (`T55–T59`)
    - `TC-own-car-cost.md` — расчёт стоимости/времени на своём авто (`T60–T65`)

- 🐞 **Баг-репорты**
  - 📁 [`bugreports/`](bugreports)
  - Вкладка Google Sheets: «Этап 4. Баг-репорты»
  - Критические дефекты:
    - `BUG2`, `BUG3`, `BUG4`, `BUG6`, `BUG7`, `BUG11`, `BUG14`, `BUG15`, `BUG16`

## Итоги тестирования

> Значения ниже подставь из своей Google-таблицы, когда завершишь перенос всех кейсов.

- Всего тест-кейсов: **N**  
  - 🟢 Passed: **X**  
  - 🔴 Failed: **Y**  

- Всего багов: **16**  
  - Критических: **…**  
  - Желательных: **…**

**Вывод:** из‑за ошибок в валидации полей (Часы/Минуты/Откуда/Куда) и некорректных расчётов стоимости/времени поездки релиз **не рекомендуется** до исправления критических дефектов и повторного регресса.

## Окружение

- OS: Windows 11 Pro 21H2  
- Browser: Google Chrome 144.0.7559.133

## Автор

Ельников Анатолий, когорта 53

