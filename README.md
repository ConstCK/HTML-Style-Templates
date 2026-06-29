# HTML Design Templates 2025–2026

Коллекция из **15 самодостаточных UI-тем** — каждая тема это один `index.html` с встроенным CSS и Google Fonts. Без сборки, без npm, без фреймворков.

Откройте [`index.html`](index.html) в браузере — там навигация по всем темам.

## Структура

```
HTMLDesign/
├── index.html          # главная страница со списком тем
├── 01/                 # Chrome Metallic
├── 02/                 # Soft UI Clay
├── 03/                 # Mint Fresh
├── 04/                 # Glass Frost
├── 05/                 # Bento Grid
├── 06/                 # Editorial Magazine
├── 07/                 # Dark SaaS Aurora
├── 08/                 # Neo-Brutalism
├── 09/                 # Cyberpunk Neon
├── 10/                 # Grotesque Art
├── 11/                 # Minimalist
├── 12/                 # Light SaaS
├── 13/                 # Earth Warm
├── 14/                 # Corporate Strict
└── 15/                 # AI Gradient
```

Нумерация папок **01–15** совпадает с порядком на главной странице.

## Темы

| #   | Название           | Стиль                     | Особенность контролов                                    |
| --- | ------------------ | ------------------------- | -------------------------------------------------------- |
| 01  | Chrome Metallic    | Тёмный chrome + малахит   | Metallic bezel select, glossy orbs                       |
| 02  | Soft UI Clay       | Claymorphism              | Clay orb checkbox/radio, зелёный акцент `#228653`        |
| 03  | Mint Fresh         | Wellness, мягкий мятный   | Сбалансированный тон, segmented tabs                     |
| 04  | Glass Frost        | Enterprise glassmorphism  | Backdrop blur, нейтральная палитра                       |
| 05  | Bento Grid         | iOS / Material hybrid     | Pill select, bento-layout                                |
| 06  | Editorial Magazine | Print / editorial         | Underline select, типографика                            |
| 07  | Dark SaaS Aurora   | Тёмный SaaS               | Terminal `[select]`, aurora-фон                          |
| 08  | Neo-Brutalism      | Neo-brutal agency         | Square widgets, жёсткие тени                             |
| 09  | Cyberpunk Neon     | Cyberpunk                 | Hex checkbox, diamond radio                              |
| 10  | Grotesque Art      | Экспериментальный         | Skew select, blob radio                                  |
| 11  | Minimalist         | Swiss / minimal           | Underline inputs, thin controls                          |
| 12  | Light SaaS         | Stripe-style              | Светлый SaaS, indigo-акцент                              |
| 13  | Earth Warm         | Terracotta / slow living  | Earth checkbox, pill tabs                                |
| 14  | Corporate Strict   | Строгий корпоративный B2B | Navy, IBM Plex Sans, border-left alerts, square controls |
| 15  | AI Gradient        | AI / tech 2026            | Gradient accents, glassmorphism, modern AI aesthetic     |

## Widget Kit

В каждой теме — полный набор из **13 компонентов** с уникальным стилем под эстетику темы:

- Alerts (success, warning, error, info)
- Badges
- Inputs + Textarea
- Select
- Checkboxes
- Radio
- Toggle
- Range
- Progress
- Tabs
- Pagination
- Tooltip
- Modal (`<dialog>` + JS)

Общие CSS-классы: `.widget-kit`, `.wk-*`.

### Alerts

| Тип     | Цвет                        |
| ------- | --------------------------- |
| success | зелёный (по теме)           |
| warning | оранжевый / жёлтый          |
| error   | бордовый / красный          |
| info    | нейтральный или акцент темы |

### Select

Dropdown читаем в светлых и тёмных темах: `color-scheme`, явные цвета для `<option>`.  
В ряде тем select кликается по всей области (обёртка + `showPicker()`).

### Modal

```html
<button type="button" data-open-modal="my-modal">Открыть</button>

<dialog class="modal" id="my-modal">
  <button type="button" class="modal-close modal-close-btn">×</button>
  ...
</dialog>
```

## Использование

1. Клонируйте или скопируйте нужную папку `01`–`15`.
2. Откройте `index.html` в браузере (достаточно двойного клика или Live Server).
3. Адаптируйте контент и CSS под свой проект.

Каждый файл автономен — можно деплоить как статику на любой хостинг.

## Технологии

- HTML5
- CSS3 (custom properties, flexbox, `backdrop-filter` где поддерживается)
- Vanilla JS (modal, select picker)
- Google Fonts

## Лицензия

Шаблоны для свободного использования в личных и коммерческих проектах.
