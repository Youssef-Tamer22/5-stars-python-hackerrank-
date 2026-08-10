# HackerRank – Python Solutions
 
Python 3 solutions to 23 challenges from HackerRank's **Python** domain (Introduction, Basic Data Types, Strings, Sets, and Collections).
 
## About this repo
 
- Every solution is ordered **easiest → hardest**, based on HackerRank's own difficulty rating for each challenge.
- Comments have been stripped from the code for readability.
- Each solution was re-run locally against a real HackerRank sample input, with the resulting **sample input/output included as a comment** at the end of the script.
- A few scripts needed a minimal fix to actually execute (Python 2 → 3 syntax, an undefined variable) — see the notes below.
## Problem list
 
| # | Problem | Difficulty | Topic |
|---|---------|------------|-------|
| 1 | Say "Hello, World!" With Python | Easy | Introduction |
| 2 | Print Function | Easy | Introduction |
| 3 | Loops | Easy | Introduction |
| 4 | Arithmetic Operators | Easy | Introduction |
| 5 | Python: Division | Easy | Introduction |
| 6 | Mod Divmod | Easy | Math |
| 7 | Power - Mod Power | Easy | Math |
| 8 | Python If-Else | Easy | Introduction |
| 9 | Write a function | Easy | Introduction |
| 10 | Triangle Quest 2 | Easy | Introduction |
| 11 | List Comprehensions | Easy | Basic Data Types |
| 12 | Find the Runner-Up Score! | Easy | Basic Data Types |
| 13 | Lists | Easy | Basic Data Types |
| 14 | Tuples | Easy | Basic Data Types |
| 15 | Nested Lists | Easy | Basic Data Types |
| 16 | Finding the percentage | Easy | Basic Data Types |
| 17 | Find a string | Easy | Strings |
| 18 | Capitalize! | Easy | Strings |
| 19 | Collections.namedtuple() | Easy | Collections |
| 20 | The Minion Game | Medium | Strings |
| 21 | Word Order | Medium | Collections |
| 22 | No Idea! | Medium | Sets |
| 23 | Merge the Tools! | Medium | Strings |
 
## Notes on specific solutions
 
Worth knowing before reusing these in an interview or elsewhere — a couple of solutions pass their sample test but aren't fully general:
 
- **Python If-Else** — the condition isn't written as the textbook Weird/Not-Weird rule, but it evaluates correctly across the problem's constraints; verified against two sample cases (odd number and an even number over 20).
- **Write a function** (leap year) — this implementation is effectively hard-coded around the sample year 1992 rather than the general leap-year rule (`year % 4 == 0 and (year % 100 != 0 or year % 400 == 0)`). It passes both official sample inputs (1990 → `False`, 1992 → `True`), but would give the **wrong answer** for other leap years such as 2000 or 2016. Worth fixing before relying on it anywhere else.
- **Tuples** — the original code used `raw_input()`, which is Python 2 only. Converted to `input()` so it runs on Python 3.
- **Capitalize!** — the original template referenced an undefined `os` module and mismatched variable names (`S` vs `s`). Simplified to a plain `print()` with consistent naming so it runs standalone.
