# Яндекс Маршруты — Итоговый проект 2 спринта

Репозиторий с результатами ручного тестирования веб‑сервиса **Яндекс Маршруты**: тест-анализ, классы эквивалентности и граничные значения, тест-кейсы, баг-репорты.

## Ссылки

- Сервис: https://qa-routes.praktikum-services.ru/
- Требования к сервису: https://docs.google.com/document/d/1tIs3KqK79vGR60EoGiDKLavvgsj0cjjrdSRK3AFdY6g/edit
- Рабочая тестовая таблица (Google Sheets): https://docs.google.com/spreadsheets/d/1ku3De2DZUbj_QlJKdQU7wEh0N3EIILJ8D6_vwkshmQU/edit

## Артефакты

- ✅ **Тест-анализ**
  - 📄 [`analysis/overview.md`](analysis/overview.md)
  - Вкладка Google Sheets: [«Этап 1. Тест-анализ»](https://docs.google.com/spreadsheets/d/1ku3De2DZUbj_QlJKdQU7wEh0N3EIILJ8D6_vwkshmQU/edit?gid=1610041137)

- ✅ **КЭ и ГЗ**
  - 📄 [`ce-gz/time-fields.md`](ce-gz/time-fields.md)
  - 📄 [`ce-gz/address-fields.md`](ce-gz/address-fields.md)
  - 📄 [`ce-gz/routes-and-time-intervals.md`](ce-gz/routes-and-time-intervals.md)
  - Вкладка Google Sheets: [«Этап 2. КЭ и ГЗ»](https://docs.google.com/spreadsheets/d/1ku3De2DZUbj_QlJKdQU7wEh0N3EIILJ8D6_vwkshmQU/edit?gid=1304990855)

- ✅ **Тест-кейсы**
  - 📁 [`testcases/`](testcases)
  - Вкладка Google Sheets: [«Этап 3. Тест-кейсы»](https://docs.google.com/spreadsheets/d/1ku3De2DZUbj_QlJKdQU7wEh0N3EIILJ8D6_vwkshmQU/edit?gid=1524919368)
  - Примеры групп:
    - [`TC-hours.md`](testcases/TC-hours.md) — валидация поля **Часы** (`T1–T24`)
    - [`TC-minutes.md`](testcases/TC-minutes.md) — валидация поля **Минуты** (`T25–T48`)
    - [`TC-from-address.md`](testcases/TC-from-address.md) — поле **Откуда** (`T49–T53`)
    - [`TC-to-address.md`](testcases/TC-to-address.md) — поле **Куда** (`T55–T59`)
    - [`TC-own-car-cost.md`](testcases/TC-own-car-cost.md) — расчёт стоимости/времени на своём авто (`T60–T65`)

- 🐞 **Баг-репорты**
  - 📁 [`bugreports/`](bugreports)
  - Вкладка Google Sheets: [«Этап 4. Баг-репорты»](https://docs.google.com/spreadsheets/d/1ku3De2DZUbj_QlJKdQU7wEh0N3EIILJ8D6_vwkshmQU/edit?gid=454479584)
  - Критические дефекты:
    - `BUG2`, `BUG3`, `BUG4`, `BUG6`, `BUG7`, `BUG11`, `BUG14`, `BUG15`, `BUG16`

## Итоги тестирования

- Всего тест-кейсов: **64**  
  - 🟢 Passed: **39**  
  - 🔴 Failed: **25**  

- Всего багов: **16**  
  - Критических: **9**  
  - Желательных: **7**

**Вывод:** из‑за ошибок в валидации полей (Часы/Минуты/Откуда/Куда) и некорректных расчётов стоимости/времени поездки релиз **не рекомендуется** до исправления критических дефектов и повторного регресса.

## Окружение

- OS: Windows 11 Pro 21H2  
- Browser: Google Chrome 144.0.7559.133

## Автор

Anatoly Elnikov (когорта 53)

