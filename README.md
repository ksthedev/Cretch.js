# Cretch.js

A Open-Source **JavaScript / Node.js utility library** with **120+ helper functions**, focused on productivity, readability, and code reuse.

⚠️ Cretch.js is Open-Source, but in the same way, you **CANT** change the content and use it in a monetized way, as per the MIT license

Designed to be **dependency-free**, **easy to understand**, and usable in **Node.js** and (partially) in the **browser**.

> Suitable for personal projects, plugins, Node.js scripts, CLI tools, bots, and simple web applications.

---

## 📦 Installation

For install CLI, download Cretch and use:

```bash
node installer.js
```

Now, you can use in your project folder:

```bash
cretch i
```

Using usage:

```js
const { //functions name separate por ',' } = require("./cretch\cretch.js")
```

Or all the functions:

```js
const c = require("./cretch\cretch.js")
```
---

## Math / Numbers

Utility functions for numeric operations and statistics.

| Function             | Description                     |
| -------------------- | ------------------------------- |
| `sum(...n)`          | Returns the sum of all numbers  |
| `sub(a, b)`          | Subtracts `b` from `a`          |
| `mul(...n)`          | Multiplies all numbers          |
| `div(a, b)`          | Divides `a` by `b`              |
| `mod(a, b)`          | Remainder of division           |
| `pow(a, b)`          | Exponentiation                  |
| `sqrt(n)`            | Square root                     |
| `cbrt(n)`            | Cube root                       |
| `abs(n)`             | Absolute value                  |
| `round(n)`           | Rounds to nearest integer       |
| `floor(n)`           | Rounds down                     |
| `ceil(n)`            | Rounds up                       |
| `min(...n)`          | Smallest value                  |
| `max(...n)`          | Largest value                   |
| `clamp(v, min, max)` | Restricts value to range        |
| `clamp01(v)`         | Restricts value between 0 and 1 |
| `rand(min, max)`     | Random float                    |
| `randInt(min, max)`  | Random integer                  |
| `avgMath(...n)`      | Average of values               |
| `percent(a, b)`      | Percentage of `a` over `b`      |
| `degToRad(n)`        | Degrees to radians              |
| `radToDeg(n)`        | Radians to degrees              |
| `lerp(a, b, t)`      | Linear interpolation            |
| `distance(a, b)`     | Absolute distance               |
| `factorial(n)`       | Factorial                       |
| `sign(n)`            | Number sign                     |
| `even(n)`            | Checks if even                  |
| `odd(n)`             | Checks if odd                   |
| `isInt(n)`           | Checks if integer               |
| `isFloat(n)`         | Checks if float                 |
| `median(arr)`        | Median value                    |
| `variance(arr)`      | Statistical variance            |
| `stddev(arr)`        | Standard deviation              |

---

## String Utilities

Functions for manipulating and validating strings.

| Function                  | Description                       |
| ------------------------- | --------------------------------- |
| `capitalize(str)`         | Capitalizes first letter          |
| `title(str)`              | Converts to title case            |
| `reverse(str)`            | Reverses string                   |
| `count(str, char)`        | Counts occurrences                |
| `between(str, a, b)`      | Extracts substring between values |
| `slug(str)`               | URL-friendly slug                 |
| `onlyNumbers(str)`        | Removes non-numeric chars         |
| `truncate(str, n)`        | Truncates string                  |
| `repeat(str, n)`          | Repeats string                    |
| `padLeft(str, n, char)`   | Left padding                      |
| `padRight(str, n, char)`  | Right padding                     |
| `words(str)`              | Splits into words                 |
| `isEmptyStr(str)`         | Checks if empty                   |
| `stripHtml(str)`          | Removes HTML tags                 |
| `camel(str)`              | Converts to camelCase             |
| `kebab(str)`              | Converts to kebab-case            |
| `snake(str)`              | Converts to snake_case            |
| `startsWithAny(str, arr)` | Starts with any prefix            |
| `endsWithAny(str, arr)`   | Ends with any suffix              |
| `isEmail(str)`            | Email validation                  |
| `isUrl(str)`              | URL validation                    |

---

## Array Utilities

Common helpers for array manipulation.

| Function           | Description            |
| ------------------ | ---------------------- |
| `first(arr)`       | First element          |
| `last(arr)`        | Last element           |
| `unique(arr)`      | Removes duplicates     |
| `chunk(arr, n)`    | Splits into chunks     |
| `shuffle(arr)`     | Randomizes order       |
| `sumArr(arr)`      | Sum of values          |
| `avg(arr)`         | Average                |
| `range(n)`         | Creates range array    |
| `randomItem(arr)`  | Random element         |
| `flatten(arr)`     | Flattens nested arrays |
| `compact(arr)`     | Removes falsy values   |
| `difference(a, b)` | Array difference       |
| `intersect(a, b)`  | Array intersection     |
| `groupBy(arr, fn)` | Groups by function     |

---

## Object Utilities

Helpers for object manipulation.

| Function                | Description      |
| ----------------------- | ---------------- |
| `keys(obj)`             | Object keys      |
| `values(obj)`           | Object values    |
| `clone(obj)`            | Shallow clone    |
| `deepClone(obj)`        | Deep clone       |
| `merge(a, b)`           | Merges objects   |
| `pick(obj, keys)`       | Picks properties |
| `omit(obj, keys)`       | Omits properties |
| `get(obj, path, def)`   | Safe getter      |
| `set(obj, path, value)` | Deep setter      |
| `has(obj, path)`        | Checks existence |
| `mapValues(obj, fn)`    | Maps values      |
| `deepEqual(a, b)`       | Deep comparison  |

---

## DOM Utilities (Browser)

> ⚠️ Available **only in browser environments**

| Function             | Description      |
| -------------------- | ---------------- |
| `qs(sel, parent)`    | querySelector    |
| `qsa(sel, parent)`   | querySelectorAll |
| `on(el, event, fn)`  | addEventListener |
| `css(el, obj)`       | Applies styles   |
| `hide(el)`           | display: none    |
| `show(el, type)`     | Shows element    |
| `html(el, value)`    | innerHTML        |
| `text(el, value)`    | textContent      |
| `addClass(el, c)`    | Adds class       |
| `remClass(el, c)`    | Removes class    |
| `toggleClass(el, c)` | Toggles class    |
| `create(tag, props)` | Creates element  |
| `ready(fn)`          | DOM ready        |

---

## Node.js / System

Node-specific helpers for filesystem, OS, and processes.

| Function                | Description            |
| ----------------------- | ---------------------- |
| `exists(path)`          | Path exists            |
| `read(file)`            | Reads file             |
| `write(file, content)`  | Writes file            |
| `append(file, content)` | Appends file           |
| `remove(path)`          | Removes file/folder    |
| `mkdir(path)`           | Creates directory      |
| `list(dir)`             | Lists directory        |
| `copy(src, dest)`       | Copies file            |
| `move(src, dest)`       | Moves file             |
| `exec(cmd)`             | Executes shell command |
| `spawnCmd(cmd, args)`   | Spawns process         |
| `sleep(ms)`             | Async delay            |
| `uuid()`                | UUID v4                |
| `hash(text, algo)`      | Hash generator         |
| `jsonRead(file)`        | Reads JSON             |
| `jsonWrite(file, obj)`  | Writes JSON            |
| `prompt(text)`          | CLI input              |
| `cwd()`                 | Current directory      |
| `platform()`            | OS platform            |
| `home()`                | Home directory         |
| `tmp()`                 | Temp directory         |
| `bytesToKB(b)`          | Bytes to KB            |
| `bytesToMB(b)`          | Bytes to MB            |
| `toBool(v)`             | Converts to boolean    |
| `debounce(fn, ms)`      | Debounce function      |
| `throttle(fn, ms)`      | Throttle function      |
| `noop()`                | Empty function         |
| `log(...args)`          | console.log shortcut   |

---

## Philosophy

* Zero dependencies
* Small, focused functions
* Readable source code
* Easy to extend and customize

---

## License

MIT

---

Developed by **ksdev**.

> “When the language does not provide it, the library solves it.”
