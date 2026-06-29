# translitua

Ukrainian-to-Latin transliteration tool for names and toponyms.

Single HTML file — no dependencies, no server required. Also includes Adobe JSX scripts for Illustrator and InDesign.

---

[English](#english) · [Українська](#ukrainian)

---

## English

### What it does

Converts Ukrainian text (names, surnames, toponyms) to Latin script using two standards:

- **A3 / UKPPT 1996** — geographic transliteration with simplified rules (no apostrophes, no `iie`/`iia` duplications, `ьо` → `io`)
- **KMU 2010** — official standard approved by Cabinet of Ministers resolution №55, 27 January 2010

### Web App

Open `index.html` in any browser — no installation, no server, no dependencies.

- Switch between A3 and KMU 2010 with the mode buttons at the top
- Type Ukrainian text on the left — transliteration appears on the right in real time
- **Copy** button copies the result to clipboard
- **Clear** button resets the input
- Character count shown below each field
- Input is saved to `localStorage` between sessions

### Adobe Scripts

JSX scripts for in-place transliteration directly inside Adobe applications:

| Script | Application | Standard |
|--------|-------------|----------|
| `scripts/A3 Translit (AI).jsx` | Adobe Illustrator | A3 / UKPPT 1996 |
| `scripts/A3 Translit (ID).jsx` | Adobe InDesign | A3 / UKPPT 1996 |
| `scripts/Translit KMU 2010 (AI).jsx` | Adobe Illustrator | KMU 2010 |
| `scripts/Translit KMU 2010 (ID).jsx` | Adobe InDesign | KMU 2010 |

Select text, run the script — works with point text, text frames, and text on a path.

**Installation — Illustrator:**
Place the `.jsx` file in:
- macOS: `Applications/Adobe Illustrator <version>/Presets/en_GB/Scripts/`
- Windows: `C:\Program Files\Adobe\Adobe Illustrator <version>\Presets\en_US\Scripts\`

**Installation — InDesign:**
Open `Window > Utilities > Scripts`, right-click the `User` folder → `Reveal in Finder / Explorer`, place the `.jsx` file there.

### Files

```
translitua/
├── index.html        # Web app — all-in-one, no external dependencies
└── scripts/
    ├── A3 Translit (AI).jsx          # Illustrator — A3 standard
    ├── A3 Translit (ID).jsx          # InDesign — A3 standard
    ├── Translit KMU 2010 (AI).jsx    # Illustrator — KMU 2010
    └── Translit KMU 2010 (ID).jsx    # InDesign — KMU 2010
```

### Credits

JSX scripts based on [a3-tools](https://github.com/agentyzmin/a3-tools) by [Агенти змін](http://translit.a3.kyiv.ua), author Олександр Колодько.

---

## Ukrainian

### Що це

Інструмент для транслітерації українських імен та топонімів латиницею. Підтримує два стандарти:

- **A3 / УКППТ 1996** — географічна транслітерація зі спрощеними правилами (без апострофів, без дублювань «iie»/«iia», «ьо» → «io»)
- **КМУ 2010** — офіційна транслітерація, затверджена [постановою](https://zakon.rada.gov.ua/laws/show/55-2010-%D0%BF) КМУ №55 від 27 січня 2010 р.

### Веб-застосунок

Відкрийте `index.html` у будь-якому браузері — без встановлення, без сервера, без залежностей.

- Перемикання між A3 і КМУ 2010 кнопками зверху
- Введіть текст ліворуч — транслітерація з'являється праворуч у реальному часі
- Кнопка **«Копіювати»** — копіює результат у буфер обміну
- Кнопка **«Очистити»** — скидає поле введення
- Лічильник символів під кожним полем
- Введений текст зберігається у `localStorage` між сесіями

### Скрипти для Adobe

JSX-скрипти для транслітерації безпосередньо в Adobe-додатках:

| Скрипт | Програма | Стандарт |
|--------|----------|----------|
| `scripts/A3 Translit (AI).jsx` | Adobe Illustrator | A3 / УКППТ 1996 |
| `scripts/A3 Translit (ID).jsx` | Adobe InDesign | A3 / УКППТ 1996 |
| `scripts/Translit KMU 2010 (AI).jsx` | Adobe Illustrator | КМУ 2010 |
| `scripts/Translit KMU 2010 (ID).jsx` | Adobe InDesign | КМУ 2010 |

Виберіть текст, запустіть скрипт. Працює з точковим текстом, текстовими фреймами, текстом на кривих.

**Встановлення — Illustrator:**
Збережіть `.jsx` у папку:
- macOS: `Applications/Adobe Illustrator <версія>/Presets/en_GB/Scripts/`
- Windows: `C:\Program Files\Adobe\Adobe Illustrator <версія>\Presets\en_US\Scripts\`

**Встановлення — InDesign:**
Відкрийте `Window > Utilities > Scripts`, правою кнопкою на папці `User` → `Reveal in Finder / Explorer`, помістіть туди `.jsx`.

### Подяки

JSX-скрипти засновані на [a3-tools](https://github.com/agentyzmin/a3-tools) від [Агентів змін](http://translit.a3.kyiv.ua), автор Олександр Колодько.
