# Skill: Code Review (Internship-Level)

## Purpose
Review Ali's code for internship readiness. Be direct — flag real issues, don't sugarcoat.

## How to Invoke
Paste code and say: "review this" or "code review" or reference this file.

---

## Review Process (5 Passes)

### Pass 1 — Correctness
- Does it do what it's supposed to do?
- Are edge cases handled? (null, empty input, negative numbers, boundary values)
- Any logic bugs or off-by-one errors?

### Pass 2 — Readability
- Are variable and method names descriptive? (`userScores` not `data`)
- Does each function do one thing?
- Are magic numbers replaced with named constants?
- Is the code easy to follow without comments?

### Pass 3 — Cleanliness
- Remove dead code, commented-out blocks, unused imports
- No redundant logic or copy-paste
- Consistent formatting and indentation

### Pass 4 — Robustness
- Input validation where needed
- No swallowed exceptions or empty catch blocks
- No silent failures that would be hard to debug in prod

### Pass 5 — Internship Signal
- Would a senior engineer need to ask "why?" anywhere?
- Is the structure explainable in an interview?
- Does it show understanding of tradeoffs, not just a working solution?
- Does it follow conventions for the language being used?

---

## Output Format

Flag issues by severity:
- **fix** — blocks clean, professional code. Must change.
- **improve** — matters in an interview or code review context. Should change.
- **note** — optional polish. Worth knowing but not critical.

End with a one-line verdict: what level this code reads at and the single highest-impact thing to fix.

---

## Language-Specific Reminders
- **JavaScript**: use single quotes, not double quotes
- **Java**: follow standard naming conventions (camelCase methods, PascalCase classes)
- **Python**: follow PEP 8; prefer list comprehensions over verbose loops where readable
