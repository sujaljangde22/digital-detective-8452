# Mission 5 — Numbers and Data

## Task / Objective

Convert numbers between decimal, binary and hexadecimal, verify the results with Python, and explain how computers store text.

## Work Completed

### Task 5.1 — Convert numbers by hand

| Conversion | Working | Answer |
|---|---|---|
| Decimal `13` to binary | `13 = 8 + 4 + 1`. The bits for `8, 4, 2, 1` are `1, 1, 0, 1`. | `1101` |
| Decimal `25` to binary | `25 = 16 + 8 + 1`. The bits for `16, 8, 4, 2, 1` are `1, 1, 0, 0, 1`. | `11001` |
| Binary `1010` to decimal | `1 × 8 + 0 × 4 + 1 × 2 + 0 × 1 = 10` | `10` |
| Binary `1101` to decimal | `1 × 8 + 1 × 4 + 0 × 2 + 1 × 1 = 13` | `13` |
| Hexadecimal `A` to decimal | `A` represents ten. | `10` |
| Hexadecimal `1F` to decimal | `1 × 16 + 15 = 31` | `31` |
| Binary `1111` to hexadecimal | `8 + 4 + 2 + 1 = 15`. In hexadecimal, `15` is `F`. | `F` |

### Task 5.2 — Verify using Python

| Expression | Result | Matches my calculation |
|---|---|---|
| `bin(13)` | `'0b1101'` | Yes |
| `bin(25)` | `'0b11001'` | Yes |
| `int("1010", 2)` | `10` | Yes |
| `int("1101", 2)` | `13` | Yes |
| `int("A", 16)` | `10` | Yes |
| `int("1F", 16)` | `31` | Yes |
| `hex(15)` | `'0xf'` | Yes |

### Task 5.3 — Build and test a number converter

I created `number_converter.py` to read a decimal integer and display it in binary and hexadecimal.

| Input | Binary output | Hexadecimal output |
|---:|---|---|
| 7 | `0b111` | `0x7` |
| 25 | `0b11001` | `0x19` |
| 42 | `0b101010` | `0x2a` |

### Task 5.4 — How text is stored

The ASCII decimal code for `A` is `65`, and the code for `a` is `97`. An encoding gives programs a shared rule for turning text into bytes and reading those bytes back as text. The rupee sign `₹` is outside basic ASCII and can be stored using UTF-8.

## Commands / Tools Used

- `python3` opened the interactive Python prompt.
- `python3 mission-05-numbers-data/number_converter.py` ran my converter from the repository folder.
- `input()` read the number as text. `int()` converted it into an integer and let me read binary or hexadecimal text by specifying its base.
- `bin()` returned the binary representation with a `0b` prefix. `hex()` returned the hexadecimal representation with a `0x` prefix.
- `ord()` displayed the numeric code for each letter. `.encode("utf-8")` converted a character to UTF-8 bytes.

## My Understanding

The same number can be written in several bases. In binary, each place is a power of two. In hexadecimal, each place is a power of sixteen. Python’s prefixes make it easy to recognize which base a result uses.

## Difficulties Faced

No major difficulties.

## How I Resolved Them

Not applicable.

## Evidence / Files

- `number_converter.py` contains my program.
- This README records my hand calculations, Python checks and converter results.

## Commit Details

- Commit message: `Complete number conversions and text encoding`
- Push status: Verified on GitHub (commit `f93da8c`).