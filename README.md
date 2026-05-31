# 🕐 Widget Mond — macOS виджет даты и времени / macOS Date & Time Widget

---

## 🇷🇺 Русский

### 📖 Что это?

**Mond** — это набор виджетов для программы **Übersicht** (macOS), которые показывают на рабочем столе текущий день недели, дату и время. Всё выглядит стильно и минималистично. 👨‍💻

Особенности:
- 🎨 Красивый декоративный шрифт **Anurati** для заголовка дня недели
- 📐 Настраиваемое положение на экране
- 🎭 Множество готовых вариантов на любой вкус
- 🇷🇺 Есть конфигурации с русскими названиями дней и месяцев
- 🕹 Лёгкое переключение между вариантами

---

### ⚙️ Как установить Übersicht

Übersicht — это бесплатная программа для macOS, которая позволяет запускать виджеты на рабочем столе.

#### 🍺 Вариант 1: через Homebrew (рекомендую)

Откройте **Терминал** (`Cmd + Пробел` → введите `Терминал` / `Terminal`) и выполните команду:

```bash
brew install --cask ubersicht
```

> Если Homebrew ещё не установлен — сначала установите его одной командой из терминала:  
> `https://brew.sh` (скопируйте команду с сайта и вставьте в Терминал)

#### 🌐 Вариант 2: скачать с официального сайта

1. Зайдите на сайт: [http://tracesof.net/uebersicht/](http://tracesof.net/uebersicht/)
2. Нажмите **Download** ⬇️
3. Откройте скачанный `.dmg` файл
4. Перетащите **Übersicht** в папку **Программы (Applications)** 📂
5. Запустите Übersicht из Launchpad или папки Программы

Когда Übersicht запустится, в строке меню (сверху справа) появится иконка в виде четырёх квадратиков **⬛⬛⬛⬛**.

---

### 🔤 Как установить шрифт Anurati

В папке **Mond** есть файл `Anurati.otf` — это красивый декоративный шрифт. Его нужно установить:

1. Откройте папку **widget-Mond** в Finder
2. Дважды кликните по файлу **Anurati.otf** 👆
3. Откроется приложение **Шрифты (Font Book)**
4. Нажмите кнопку **Установить шрифт** ✅
5. Готово! Шрифт установлен на системном уровне

> ⚠️ **Важно**: шрифт Anurati поддерживает только **ЗАГЛАВНЫЕ буквы (A-Z)**. Это дизайнерское решение — он специально сделан для коротких заголовков. Строчные буквы он будет игнорировать.

---

### 📦 Как установить виджет

1. Скопируйте папку **widget-Mond** куда-нибудь (например, на Рабочий стол) 📋
2. Нажмите на иконку Übersicht в строке меню → выберите **Open Widgets Folder** 📂
   - Или в Finder нажмите `Cmd + Shift + G` и вставьте путь:  
     `~/Library/Application Support/Übersicht/widgets/`
3. Перетащите папку **widget-Mond** в открывшуюся папку **widgets** 🚚
4. Снова нажмите на иконку Übersicht → выберите **Refresh** 🔄
5. В меню Übersicht появится раздел **widget-Mond** со списком всех конфигураций
6. Нажмите **Enable** напротив той конфигурации, которую хотите включить (например, `mond-classic`) ✅

🎉 Виджет появится на рабочем столе!

> 💡 **Совет**: вы можете включить сразу несколько конфигураций одновременно — они будут отображаться все вместе на экране.

---

### 🎨 Как выбрать конфигурацию

Все файлы разложены по папкам. Вот полный список:

#### 📁 `originalMonds/` — Базовые версии

| Файл | Описание |
|---|---|
| `mond-classic.jsx` | Классический вид: день недели (крупно), дата, время |
| `mond-classic-v2.jsx` | То же, но с декоративными символами 愛 и 狂熱 |
| `mond-russian.jsx` | 📌 **Дни недели и месяцы на русском языке** |
| `mond-all-Russian.jsx` | То же самое, что и выше |

#### 📁 `locale/` — Разные форматы даты

| Файл | Описание |
|---|---|
| `mond-24h.jsx` | Время в 24-часовом формате (18:30 вместо 6:30 PM) |
| `mond-europe.jsx` | Дата в европейском формате: **дд.мм.гггг** |
| `mond-iso.jsx` | Дата в международном формате: **гггг-мм-дд** |
| `mond-ordinal.jsx` | Английские окончания: January **1st**, May **17th** |

#### 📁 `minimal/` — Минималистичные варианты

| Файл | Описание |
|---|---|
| `mond-simple.jsx` | Без шрифта Anurati — обычный Helvetica, строгий вид |
| `mond-small.jsx` | Маленький виджет в правом верхнем углу 📐 |
| `mond-thin.jsx` | Тонкий шрифт (font-weight: 100), очень воздушный |

#### 📁 `style/` — Разные стили оформления

| Файл | Описание |
|---|---|
| `mond-reverse.jsx` | Перевёрнутый: **время** крупно сверху, день снизу |
| `mond-divider.jsx` | С разделительной горизонтальной линией ➖ |
| `mond-brackets.jsx` | Дата в квадратных скобках: **[17 MAЯ, 2026]** |
| `mond-compact.jsx` | Компактный: день и время в одной строке |
| `mond-lowercase.jsx` | Строчные буквы (не ЗАГЛАВНЫЕ) |

#### 📁 `partial/` — Показывать частично

| Файл | Описание |
|---|---|
| `mond-no-date.jsx` | Без даты (только день недели + время) |
| `mond-no-day.jsx` | Без дня недели (только дата + время) |
| `mond-no-time.jsx` | Без времени (только день + дата) |
| `mond-only-day.jsx` | **Только** день недели (самый крупный, 6vw) |
| `mond-only-time.jsx` | **Только** время (крупно) |

#### 📁 `social/` — С иконками социальных сетей

| Файл | Описание |
|---|---|
| `mond-social.jsx` | Полный виджет + иконки GitHub, Telegram, YouTube, Discord, Twitter |
| `mond-social-mini.jsx` | Только время + иконки |
| `mond-social-ru.jsx` | 📌 **Русский язык + иконки соцсетей** |

---

### 🔧 Как настроить виджет (для чайников)

#### 📍 Как изменить положение на экране

1. Откройте нужный `.jsx` файл — кликните по нему правой кнопкой → **Открыть в приложении** → выберите **TextEdit** (на Mac) или любой редактор (хоть Блокнот)
2. Найдите в начале файла такие строки:

```css
top: 20%;
left: 50%;
transform: translate(-50%, -50%);
```

Это координаты виджета.

**Что можно менять:**

- `top` — отступ **сверху**. Чем больше число, тем ниже виджет. Можно писать в процентах (`%`) или пикселях (`px`)
  - `top: 0%` — в самом верху
  - `top: 50%` — по центру по вертикали
  - `top: 90%` — почти в самом низу
  
- `left` — отступ **слева**
  - `left: 50%` — по центру по горизонтали
  - `left: 5%` — ближе к левому краю

- `transform: translate(-50%, -50%)` — центрирование. Когда стоит `left: 50%`, эта строчка центрирует виджет ровно посередине. Если хотите привязать к углу — замените на `transform: none`

**Готовые варианты расположения:**

```
По центру экрана:
  top: 50%;  left: 50%;  transform: translate(-50%, -50%);

Левый верхний угол:
  top: 5%;  left: 5%;  transform: none;

Правый верхний угол:
  top: 5%;  left: auto;  right: 5%;  transform: none;

Внизу по центру:
  top: 85%;  left: 50%;  transform: translate(-50%, -50%);
```

После сохранения файла нажмите иконку Übersicht → **Refresh** 🔄

> 💡 **Лайфхак**: В Übersicht можно просто зажать `Cmd` и перетащить виджет мышкой в любое место. Новые координаты применятся сразу! После перетаскивания их можно посмотреть и сохранить в файл.

---

#### 🎨 Как изменить цвет текста

Найдите в `.jsx` файле:

```css
color: #f7f3e8;
```

Замените `#f7f3e8` на любой другой цвет:

| Код | Цвет |
|---|---|
| `#ffffff` | ⬜ Белый |
| `#000000` | ⬛ Чёрный |
| `#ff0000` | 🔴 Красный |
| `#00ff00` | 🟢 Зелёный |
| `#0088ff` | 🔵 Синий |
| `#ff8800` | 🟠 Оранжевый |
| `#ff00ff` | 🟣 Розовый |
| `#888888` | ⬜ Серый |

> 🎨 **Где брать коды цветов**: загуглите «color picker» — есть куча сайтов, где можно выбрать цвет и скопировать его код вида `#rrggbb`.

Цвет можно задать и так: `color: white` / `color: black` / `color: red` (английскими словами).

**Тень текста** (придаёт объём):

```css
text-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
```

- Первое число — смещение по горизонтали (`0` — нет)
- Второе — смещение по вертикали
- Третье — размытие (чем больше, тем более размытая тень)
- Четвёртое (`rgba`) — цвет тени с прозрачностью (последнее число — прозрачность от 0 до 1)

Сохраните файл → **Refresh** в Übersicht.

---

#### 🔤 Как изменить размер шрифта

Размер шрифта задаётся в **vw** (процент от ширины экрана). Найдите:

```css
font-size: 5vw;
```

- `5vw` = 5% от ширины экрана
- `2vw` — мелко
- `10vw` — очень крупно

Шрифт дня и даты/времени можно менять отдельно:

```css
.day {
  font-size: 5vw;  /* день недели */
}

.date {
  font-size: 1.5vw;  /* дата */
}

.time {
  font-size: 1.2vw;  /* время */
}
```

Можно указать размер в пикселях: `font-size: 48px`

---

#### ⏱ Как изменить частоту обновления

Найдите в файле:

```javascript
export const refreshFrequency = 59000;
```

Число — это миллисекунды:
- `59000` = обновление раз в 59 секунд ⏱️
- `60000` = раз в минуту
- `1000` = каждую секунду 🔄
- `300000` = раз в 5 минут

> ⚠️ Не ставьте слишком часто (меньше 1000), это будет нагружать процессор.

---

#### 📝 Как изменить формат даты и времени

Найдите в файле команду:

```javascript
export const command = "date +'%A\n%d %B, %Y\n%l:%M %p'";
```

Здесь:
- `%A` — день недели (полное название, например Monday)
- `%d` — число месяца (01-31)
- `%B` — месяц (полное название, January)
- `%Y` — год (2026)
- `%l` — час (12-часовой)
- `%M` — минуты
- `%p` — AM/PM
- `\n` — перенос на новую строку

**Примеры:**

```
Только время:        date +'%l:%M %p'
Только дата:         date +'%d %B %Y'
24-часовой формат:   date +'%H:%M'
День + время:        date +'%A\n%l:%M'
```

---

### 🐛 Возможные проблемы и их решение

#### ❌ Шрифт Anurati не отображается

Если вместо красивого шрифта отображается обычный или квадратики □□□:

1. Убедитесь, что вы установили `Anurati.otf` (дважды кликнуть → **Установить шрифт**)
2. Откройте `.jsx` файл в текстовом редакторе
3. Найдите и **удалите целиком** блок `@font-face { ... }` — от слова `@font-face` до закрывающей фигурной скобки `}`. Внутри этого блока — длинная строка из букв и цифр (это закодированный шрифт, base64).
4. После удаления должно остаться просто:

```css
font-family: 'Anurati', sans-serif;
```

5. Сохраните файл → **Refresh** в Übersicht

Шрифт теперь будет браться из системы (который вы установили), а не из файла. ✅

#### ❌ Виджет не появляется на экране

1. Проверьте, что папка **widget-Mond** лежит в правильной папке:  
   `~/Library/Application Support/Übersicht/widgets/`
2. Нажмите иконку Übersicht → **Refresh All**
3. Проверьте, что в меню Übersicht для нужного файла стоит **Enabled** ✅
4. Перезапустите Übersicht: иконка → **Quit** → запустите заново

#### ❌ Хочу русские дни недели

Используйте готовые файлы:
- `originalMonds/mond-russian.jsx` 🇷🇺
- `originalMonds/mond-all-Russian.jsx` 🇷🇺
- `social/mond-social-ru.jsx` 🇷🇺 (с иконками)

#### ❌ Виджет мешает кликать по рабочему столу

Нажмите на иконку Übersicht → выберите нужный виджет → отключите опцию **Click through** (или включите, если наоборот хотите, чтобы клики проходили сквозь виджет).

---

### ⌨️ Горячие клавиши Übersicht

| Действие | Сочетание |
|---|---|
| Обновить все виджеты | `Cmd + Shift + R` |
| Скрыть/показать виджеты | `Cmd + Alt + W` |
| Перетащить виджет | Зажать `Cmd` и тащить мышкой |

---

### 💾 Резервное копирование

Чтобы не потерять настройки при переустановке macOS или переходе на новый Mac:
1. Скопируйте папку `widget-Mond` на флешку или в облако ☁️
2. На новом Mac просто установите Übersicht и скопируйте папку обратно в `~/Library/Application Support/Übersicht/widgets/`

---

## 🇬🇧 English

### 📖 What is this?

**Mond** is a collection of widgets for **Übersicht** (macOS) that displays the current day, date, and time on your desktop. It's minimal, stylish, and fully customizable. 👨‍💻

Features:
- 🎨 Custom **Anurati** decorative font for the day heading
- 📐 Adjustable position on screen
- 🎭 Multiple ready-to-use configurations
- 🇷🇺 Russian language variants included
- 🕹 Easy switching between configurations

---

### ⚙️ How to install Übersicht

#### 🍺 Option 1: via Homebrew (recommended)

Open **Terminal** (`Cmd + Space` → type `Terminal`) and run:

```bash
brew install --cask ubersicht
```

> If you don't have Homebrew yet, install it first from: `https://brew.sh`

#### 🌐 Option 2: download from the official website

1. Go to: [http://tracesof.net/uebersicht/](http://tracesof.net/uebersicht/)
2. Click **Download** ⬇️
3. Open the `.dmg` file
4. Drag **Übersicht** into **Applications** 📂
5. Launch Übersicht from Launchpad or Applications

Übersicht will appear in the menu bar (top right) as **⬛⬛⬛⬛**.

---

### 🔤 How to install the Anurati font

1. Open the **widget-Mond** folder in Finder
2. Double-click **Anurati.otf** 👆
3. **Font Book** will open
4. Click **Install Font** ✅
5. Done!

> ⚠️ **Note**: Anurati only supports **UPPERCASE letters (A-Z)**. It's a decorative font designed for headings.

---

### 📦 How to install the widget

1. Copy the **widget-Mond** folder somewhere convenient 📋
2. Click the Übersicht icon in the menu bar → **Open Widgets Folder** 📂
   - Or in Finder press `Cmd + Shift + G` and paste:  
     `~/Library/Application Support/Übersicht/widgets/`
3. Drag **widget-Mond** into the **widgets** folder 🚚
4. Click Übersicht icon → **Refresh** 🔄
5. Find **widget-Mond** in the Übersicht menu
6. Click **Enable** on the config you want (e.g., `mond-classic`) ✅

🎉 The widget appears on your desktop!

> 💡 **Tip**: You can enable multiple configs at the same time.

---

### 🎨 Available configurations

#### 📁 `originalMonds/` — Base versions

| File | Description |
|---|---|
| `mond-classic.jsx` | Classic: day (large), date, time |
| `mond-classic-v2.jsx` | With decorative characters 愛 and 狂熱 |
| `mond-russian.jsx` | 📌 **Days and months in Russian** |
| `mond-all-Russian.jsx` | Same as above |

#### 📁 `locale/` — Date formats

| File | Description |
|---|---|
| `mond-24h.jsx` | 24-hour time (18:30 instead of 6:30 PM) |
| `mond-europe.jsx` | European format: **dd.mm.yyyy** |
| `mond-iso.jsx` | ISO format: **yyyy-mm-dd** |
| `mond-ordinal.jsx` | English ordinals: January **1st**, May **17th** |

#### 📁 `minimal/` — Minimal variants

| File | Description |
|---|---|
| `mond-simple.jsx` | No Anurati font — plain Helvetica |
| `mond-small.jsx` | Small widget in the top-right corner 📐 |
| `mond-thin.jsx` | Thin font (weight: 100), extra airy |

#### 📁 `style/` — Visual styles

| File | Description |
|---|---|
| `mond-reverse.jsx` | Reversed: **time** on top, day below |
| `mond-divider.jsx` | With a horizontal divider line ➖ |
| `mond-brackets.jsx` | Date in square brackets: **[17 MAY, 2026]** |
| `mond-compact.jsx` | Compact: day and time on one line |
| `mond-lowercase.jsx` | Lowercase text (not ALL CAPS) |

#### 📁 `partial/` — Partial display

| File | Description |
|---|---|
| `mond-no-date.jsx` | No date (day + time only) |
| `mond-no-day.jsx` | No day name (date + time only) |
| `mond-no-time.jsx` | No time (day + date only) |
| `mond-only-day.jsx` | **Only** the day name (large, 6vw) |
| `mond-only-time.jsx` | **Only** the time (large) |

#### 📁 `social/` — With social media icons

| File | Description |
|---|---|
| `mond-social.jsx` | Full widget + GitHub, Telegram, YouTube, Discord, Twitter/X icons |
| `mond-social-mini.jsx` | Time only + social icons |
| `mond-social-ru.jsx` | 📌 **Russian language + social icons** |

---

### 🔧 How to customize

#### 📍 Changing position

Open a `.jsx` file in **TextEdit** or any code editor. Find:

```css
top: 20%;
left: 50%;
transform: translate(-50%, -50%);
```

- `top` — distance from the **top** edge (higher = lower on screen)
- `left` — distance from the **left** edge
- `transform: translate(-50%, -50%)` — centers the widget

**Preset positions:**

```
Center screen:
  top: 50%;  left: 50%;  transform: translate(-50%, -50%);

Top-left:
  top: 5%;  left: 5%;  transform: none;

Top-right:
  top: 5%;  left: auto;  right: 5%;  transform: none;

Bottom center:
  top: 85%;  left: 50%;  transform: translate(-50%, -50%);
```

Save → **Refresh** in Übersicht 🔄

> 💡 **Pro tip**: Hold `Cmd` and drag the widget with your mouse to reposition it visually!

---

#### 🎨 Changing color

Find this in the `.jsx` file:

```css
color: #f7f3e8;
```

Replace `#f7f3e8` with any color:

| Code | Color |
|---|---|
| `#ffffff` | ⬜ White |
| `#000000` | ⬛ Black |
| `#ff0000` | 🔴 Red |
| `#00ff00` | 🟢 Green |
| `#0088ff` | 🔵 Blue |
| `#ff8800` | 🟠 Orange |
| `#ff00ff` | 🟣 Pink |
| `#888888` | ⬜ Gray |

**Text shadow** (adds depth):

```css
text-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
```

Save → **Refresh**.

---

#### 🔤 Changing font size

Font sizes are in `vw` (percent of screen width):

```css
font-size: 5vw;
```

- `5vw` = 5% of screen width
- Each section (`.day`, `.date`, `.time`) has its own size. Adjust them individually!

---

#### ⏱ Changing refresh rate

Find:

```javascript
export const refreshFrequency = 59000;
```

- `59000` = every 59 seconds ⏱️
- `1000` = every second 🔄
- `300000` = every 5 minutes

> ⚠️ Don't set it below 1000ms (1 second) — it will waste CPU.

---

#### 📝 Changing date/time format

Find:

```javascript
export const command = "date +'%A\n%d %B, %Y\n%l:%M %p'";
```

Format specifiers:
- `%A` — full weekday name
- `%d` — day of month (01-31)
- `%B` — full month name
- `%Y` — year (2026)
- `%l` — hour (12-hour)
- `%M` — minutes
- `%p` — AM/PM
- `\n` — new line

---

### 🐛 Troubleshooting

#### ❌ Anurati font not showing

1. Make sure you installed `Anurati.otf` (double-click → **Install Font**)
2. Open the `.jsx` file in a text editor
3. **Delete** the entire `@font-face { ... }` block (from `@font-face` to the closing `}`)
4. Keep just:

```css
font-family: 'Anurati', sans-serif;
```

5. Save → **Refresh** ✅

#### ❌ Widget not appearing

1. Check that **widget-Mond** is in: `~/Library/Application Support/Übersicht/widgets/`
2. Click Übersicht icon → **Refresh All**
3. Make sure the config is **Enabled** ✅
4. Restart Übersicht: icon → **Quit** → launch again

#### ❌ I want Russian days/months

Use one of these:
- `originalMonds/mond-russian.jsx` 🇷🇺
- `originalMonds/mond-all-Russian.jsx` 🇷🇺
- `social/mond-social-ru.jsx` 🇷🇺 (with icons)

#### ❌ Widget blocks clicks on desktop

Click Übersicht icon → select the widget → toggle **Click through**.

---

### ⌨️ Übersicht Keyboard Shortcuts

| Action | Shortcut |
|---|---|
| Refresh all widgets | `Cmd + Shift + R` |
| Toggle widgets visibility | `Cmd + Alt + W` |
| Drag widget | Hold `Cmd` + drag |

---

### 💾 Backup

To save your setup:
1. Copy the `widget-Mond` folder to a USB drive or cloud ☁️
2. On a new Mac: install Übersicht → copy the folder back to `~/Library/Application Support/Übersicht/widgets/`

---

Made with ❤️ for macOS. Enjoy your desktop widgets! 🎉
