# translitua

Ukrainian-to-Latin transliteration tool for names and toponyms.

Provides two transliteration standards and Adobe scripts for Illustrator and InDesign.

---

[English](#english) · [Українська](#ukrainian)

---

## English

### What it does

Converts Ukrainian text (names, surnames, toponyms) to Latin script using two standards:

- **A3 / UKPPT 1996** — geographic transliteration with simplified rules (no apostrophes, no `iie`/`iia` duplications, `ьо` → `io`)
- **KMU 2010** — official Ukrainian transliteration standard approved by Cabinet of Ministers resolution №55, 27 January 2010

### Web App

Open `index.html` in a browser — no server required.

Type Ukrainian text on the left, get the transliteration on the right in real time. Input is saved to `localStorage` between sessions.

### Adobe Scripts

JSX scripts for in-place transliteration directly inside Adobe applications:

| Script | Application |
|--------|-------------|
| `scripts/A3 Translit (AI).jsx` | Adobe Illustrator |
| `scripts/A3 Translit (ID).jsx` | Adobe InDesign |
| `scripts/Translit KMU 2010 (AI).jsx` | Adobe Illustrator |
| `scripts/Translit KMU 2010 (ID).jsx` | Adobe InDesign |

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
├── index.html             # Web app
├── app.js                 # Transliteration logic (A3 standard)
├── style.css
├── bootstrap.min.css
├── bootstrap.min.js
├── jquery-3.2.1.min.js
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
- **КМУ 2010** — офіційна транслітерація українського алфавіту латиницею, затверджена [постановою](https://zakon.rada.gov.ua/laws/show/55-2010-%D0%BF) Кабінету Міністрів України №55 від 27 січня 2010 р.

### Веб-застосунок

Відкрийте `index.html` у браузері — сервер не потрібен.

Введіть текст ліворуч — транслітерація з'являється праворуч у реальному часі. Введений текст зберігається у `localStorage` між сесіями.

### Скрипти для Adobe

JSX-скрипти для транслітерації безпосередньо в Adobe-додатках:

| Скрипт | Програма |
|--------|----------|
| `scripts/A3 Translit (AI).jsx` | Adobe Illustrator |
| `scripts/A3 Translit (ID).jsx` | Adobe InDesign |
| `scripts/Translit KMU 2010 (AI).jsx` | Adobe Illustrator |
| `scripts/Translit KMU 2010 (ID).jsx` | Adobe InDesign |

Виберіть текст, запустіть скрипт. Працює з точковим текстом, текстовими фреймами, текстом на кривих.

**Встановлення — Illustrator:**
Збережіть `.jsx` у папку:
- macOS: `Applications/Adobe Illustrator <версія>/Presets/en_GB/Scripts/`
- Windows: `C:\Program Files\Adobe\Adobe Illustrator <версія>\Presets\en_US\Scripts\`

**Встановлення — InDesign:**
Відкрийте `Window > Utilities > Scripts`, правою кнопкою на папці `User` → `Reveal in Finder / Explorer`, помістіть туди `.jsx`.

### Подяки

JSX-скрипти засновані на [a3-tools](https://github.com/agentyzmin/a3-tools) від [Агентів змін](http://translit.a3.kyiv.ua), автор Олександр Колодько.
