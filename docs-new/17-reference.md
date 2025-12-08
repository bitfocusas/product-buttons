# Reference

## Expression Functions

Use these functions in expression mode to transform and manipulate values.

### Number Operations

| Function | Description |
|----------|-------------|
| `round(v)` | Rounds `v` to nearest integer using `Math.round` |
| `floor(v)` | Floors `v` to the nearest lower integer using `Math.floor` |
| `ceil(v)` | Ceils `v` to the nearest higher integer using `Math.ceil` |
| `abs(v)` | Returns absolute value of `v` using `Math.abs` |
| `fromRadix(v, radix)` | Parses `v` as integer in base `radix` (default `10`) |
| `toRadix(v, radix)` | Converts `v` to string in base `radix` (default `10`) |
| `toFixed(v, dp)` | Formats `v` with `dp` decimal places (minimum `0`, default `0`) |
| `isNumber(v)` | Returns `true` if `v` is not `NaN` |
| `max(...args)` | Returns largest value from arguments |
| `min(...args)` | Returns smallest value from arguments |
| `randomInt(min = 0, max = 10)` | Returns a random integer in `[min, max]` |
| `log(v)` | Returns natural logarithm of `v` |
| `log10(v)` | Returns base-10 logarithm of `v` |

### String Operations

| Function | Description |
|----------|-------------|
| `trim(v)` | Converts `v` to string and trims whitespace |
| `strlen(v)` | Returns length of string representation of `v` |
| `substr(str, start, end)` | Returns substring from `start` to `end` |
| `split(str, separator)` | Splits string by `separator` |
| `join(arr = [], separator = ',')` | Joins array values into string with `separator` |
| `concat(...strs)` | Concatenates all arguments into one string |
| `includes(str, arg)` | Returns `true` if `arg` exists within `str` |
| `indexOf(str, arg, offset)` | Returns index of `arg` starting from `offset` |
| `lastIndexOf(str, arg, offset)` | Returns last index of `arg` (optional `offset`) |
| `toUpperCase(str)` | Converts string to uppercase |
| `toLowerCase(str)` | Converts string to lowercase |
| `replaceAll(str, find, replace)` | Replaces all occurrences of `find` with `replace` |
| `decode(str, enc = 'latin1')` | Decodes `str` from `enc` into `'latin1'` using Node Buffer |
| `encode(str, enc = 'latin1')` | Encodes `str` to `enc` using Node Buffer |

### Boolean Operations

| Function | Description |
|----------|-------------|
| `bool(v)` | Returns `true` if `v` is truthy and not `'false'`/`'0'` |

### Object / JSON Operations

| Function | Description |
|----------|-------------|
| `jsonpath(obj, path)` | Evaluates JSONPath on `obj`. If `obj` is string, tries `JSON.parse`. Returns result or stringified object if parsed from string |
| `jsonparse(str)` | Safely parses JSON string, returns `null` on error |
| `jsonstringify(obj)` | Safely stringifies object, returns `null` on error |

### Time Operations

| Function | Description |
|----------|-------------|
| `unixNow()` | Returns current timestamp in milliseconds |
| `timestampToSeconds(str)` | Converts `"HH:MM:SS"` to total seconds. Returns `0` if invalid |
| `secondsToTimestamp(v, type?)` | Converts seconds to `"HH:MM:SS"`. Uses `type` format to selectively include `HH`, `mm`, `ss` |
| `msToTimestamp(v, type?)` | Converts milliseconds to timestamp (`MM:SS.d` default). Supports fractional formatting `.ms`, `.S`, `.SS`, `.SSS` |
| `timeOffset(time, offset, hr12 = false)` | Offsets a given `time` (`HH:MM[:SS]`) by `offset` (string or number). Returns adjusted time string |
| `timeDiff(from, to)` | Returns difference in seconds between two times (`HH:MM[:SS]` or ISO date-time). Returns `'ERR'` if invalid |

---

## Keyboard Shortcuts

Quick shortcuts for common actions in the Position Editor:

| Shortcut | Action |
|----------|--------|
| **B** | Create Button |
| **S** | Create Section |
| **Shift+S** | Create Shift Section |
| **F** | Create Folder Section |
| **R** | Create Router Section |

---

## Glossary

### Core Concepts

| Term | Definition |
|------|------------|
| **Position** | A collection of one or more Surfaces, typically aligned with a working role (e.g., Vision Mixer, Graphics) |
| **Surface** | A physical control device (Stream Deck, iPad, custom browser) connected to Buttons |
| **Canvas** | The 16×16 grid where buttons and sections are arranged |
| **Section** | A grouping of cells on the canvas that can contain buttons and have their own properties |

### Button Elements

| Term | Definition |
|------|------------|
| **Button** | A fundamental action handler that executes actions when pressed |
| **Action** | A command sent to a connection or internal function when triggered |
| **Feedback** | A visual indicator that changes button appearance based on conditions |
| **Preset** | A pre-configured button created by module authors for quick deployment |

### Section Types

| Term | Definition |
|------|------------|
| **Shift Section** | A section with two layers accessible via a toggle button |
| **Folder Section** | A section with multiple layers organized as folders and subfolders |
| **Popover** | A section that expands from a single button |
| **Shared Section** | A section that can be embedded in multiple positions |

### Advanced Features

| Term | Definition |
|------|------------|
| **Encoder** | A rotary control on Stream Deck Studio/Plus for value adjustment |
| **Repeater** | A function that automatically creates multiple buttons from a template |
| **Variable** | A named container that stores changing values |
| **Tag** | A keyword for organizing and filtering elements |
| **Cuelist** | A sequential list of cues for show execution |
| **Workflow** | Visual, node-based automation flows |

### Connections

| Term | Definition |
|------|------------|
| **Connection** | A link between Buttons and external hardware/software |
| **NMOS** | Network Media Open Specifications—2110 IP media connections |
| **Router** | System for routing audio/video signals between sources and destinations |
| **Salvo** | A saved collection of routes that can be executed together |

