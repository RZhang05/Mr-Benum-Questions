# Roman Numeral Converter
Convert **roman numerals** to **decimal numbers** (Integer Values).

🏆 Do the opposite if you dare.

## Roman Numeral Value Sheet
| Roman Numeral | Integer Value |
| :---: | :---: |
| `I` | 1 |
| `V` | 5 |
| `X` | 10 |
| `L` | 50 |
| `C` | 100 |
| `D` | 500 |
| `M` | 1000 |

### General Rules
###### Taken from [nmsu.edu](https://www.math.nmsu.edu/~pmorandi/math111f01/RomanNumerals.html)
1. Repeating a numeral **up to three times** represents addition of the number. For example, `III` represents `1 + 1 + 1 = 3`. Only `I, X, C, and M` can be repeated; `V, L, and D` cannot be, and there is no need to do so.
2. Writing numerals that **decrease from left to right** represents addition of the numbers. For example, `LX` represents `50 + 10 = 60` and `XVI` represents `10 + 5 + 1 = 16`.
3. To write a number that otherwise would take repeating of a **numeral four or more times**, there is a subtraction rule. Writing a **smaller numeral to the left of a larger numeral** represents subtraction. For example, `IV` represents `5 - 1 = 4` and `IX` represents `10 - 1 = 9`.

## Sample Run
### User Console
```
(Prompt) Enter a string of Roman Numerals:
(User) MCMXCIX
```

### Console Output
```
The value of MCMXCIX is 1999.
```

## Problem
If you want to test your code further try this problem: [What is this Roman Numeral](https://dmoj.ca/problem/dwite08c1p4)
