## ExpressionFunctions Reference

### Number Operations
| Function | Definition |
|---------|-------------|
| `round(v)` | Rounds `v` to nearest integer using `Math.round`. |
| `floor(v)` | Floors `v` to the nearest lower integer using `Math.floor`. |
| `ceil(v)` | Ceils `v` to the nearest higher integer using `Math.ceil`. |
| `abs(v)` | Returns absolute value of `v` using `Math.abs`. |
| `fromRadix(v, radix)` | Parses `v` as integer in base `radix` (default `10`). |
| `toRadix(v, radix)` | Converts `v` to string in base `radix` (default `10`). |
| `toFixed(v, dp)` | Formats `v` with `dp` decimal places (minimum `0`, default `0`). |
| `isNumber(v)` | Returns `true` if `v` is not `NaN`. |
| `max(...args)` | Returns largest value from arguments. |
| `min(...args)` | Returns smallest value from arguments. |
| `randomInt(min = 0, max = 10)` | Returns a random integer in `[min, max]`. |
| `log(v)` | Returns natural logarithm of `v`. |
| `log10(v)` | Returns base-10 logarithm of `v`. |

### String Operations
| Function | Definition |
|---------|-------------|
| `trim(v)` | Converts `v` to string and trims whitespace. |
| `strlen(v)` | Returns length of string representation of `v`. |
| `substr(str, start, end)` | Returns substring from `start` to `end`. |
| `split(str, separator)` | Splits string by `separator`. |
| `join(arr = [], separator = ',')` | Joins array values into string with `separator`. |
| `concat(...strs)` | Concatenates all arguments into one string. |
| `includes(str, arg)` | Returns `true` if `arg` exists within `str`. |
| `indexOf(str, arg, offset)` | Returns index of `arg` starting from `offset`. |
| `lastIndexOf(str, arg, offset)` | Returns last index of `arg` (optional `offset`). |
| `toUpperCase(str)` | Converts string to uppercase. |
| `toLowerCase(str)` | Converts string to lowercase. |
| `replaceAll(str, find, replace)` | Replaces all occurrences of `find` with `replace`. |
| `decode(str, enc = 'latin1')` | Decodes `str` from `enc` into `'latin1'` using Node `Buffer`. |
| `encode(str, enc = 'latin1')` | Encodes `str` to `enc` using Node `Buffer`. |

### Boolean Operations
| Function | Definition |
|---------|-------------|
| `bool(v)` | Returns `true` if `v` is truthy and not `'false'`/`'0'`. |

### Object / JSON Operations
| Function | Definition |
|---------|-------------|
| `jsonpath(obj, path)` | Evaluates JSONPath on `obj`. If `obj` is string, tries `JSON.parse`. Returns result or stringified object if parsed from string. |
| `jsonparse(str)` | Safely parses JSON string, returns `null` on error. |
| `jsonstringify(obj)` | Safely stringifies object, returns `null` on error. |

### Time Operations
| Function | Definition |
|---------|-------------|
| `unixNow()` | Returns current timestamp in milliseconds. |
| `timestampToSeconds(str)` | Converts `"HH:MM:SS"` to total seconds. Returns `0` if invalid. |
| `secondsToTimestamp(v, type?)` | Converts seconds to `"HH:MM:SS"`. Uses `type` format to selectively include `HH`, `mm`, `ss`. |
| `msToTimestamp(v, type?)` | Converts milliseconds to timestamp (`MM:SS.d` default). Supports fractional formatting `.ms`, `.S`, `.SS`, `.SSS`. |
| `timeOffset(time, offset, hr12 = false)` | Offsets a given `time` (`HH:MM[:SS]`) by `offset` (string or number). Returns adjusted time string. |
| `timeDiff(from, to)` | Returns difference in seconds between two times (`HH:MM[:SS]` or ISO date-time). Returns `'ERR'` if invalid. |