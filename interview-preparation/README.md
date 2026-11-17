# Interview Preparation

Sample strategy and question themes for TypeScript interviews (frontend, ~2 YOE focus).  
**These are thinking practice — not a guarantee of real questions.**  
Interview styles and technology change over time.

---

## What interviews actually test

Most 2 YOE interviews test TypeScript **lightly**: correctness of basic types, reading a type error, and “why use TS at all” — rarely deep generic wizardry.

```text
Weight of what gets asked
─────────────────────────
Typing component props / hooks / events   ████████████  (10, 11)
X vs Y differences                        ██████████    (03, 04, 05)
Reading a type error                      ████████      (12)
Unions, narrowing, utility types          ████████      (07, 08)
Basic generics                            █████         (09)
Advanced generics                         █             (left out on purpose)
```

---

## By experience level

### Fresher / 0–1 year

**Focus:** Clean basic types and clear “why TS”.

Must be able to explain:
- What problem TypeScript solves; types are erased at runtime
- `string`, `number`, `boolean`, arrays, tuples
- Type inference vs annotation
- `any` vs `unknown`

Practice topics: 01–04

---

### 1–3 years (primary target)

**Focus:** Modeling data and typing React.

Must be able to explain:
- `interface` vs `type`, optional and readonly properties
- Narrowing and discriminated unions
- `Partial`, `Pick`, `Omit`, `Record`
- A simple generic function (`groupBy<T>`)
- Typing props, `useState`, events, `useRef`, custom hooks, API responses
- Typing `params` / `searchParams` and a Route Handler in Next.js

Practice topics: 05–12

---

### 3–6 years

**Focus:** Design decisions and trade-offs.

Be ready to discuss:
- `enum` vs union of literals; `as const`
- Runtime validation (Zod) vs compile-time types
- When a generic is justified and when `unknown` is enough
- Keeping frontend and API types in sync

Practice topics: 03, 04, 07, 09, 11

---

## The five practice formats

| Format | Example | Where to practice |
|---|---|---|
| “Difference between X and Y” | `interface` vs `type`, `any` vs `unknown`, `enum` vs union | 03, 04, 05 |
| “What error does this give and why” | Read a broken snippet | 12 |
| Small typing task | Type an untyped function or component live | 06, 10 |
| Utility-type reasoning | “Why `Partial<T>` here?” | 08 |
| Why TypeScript | Defend its value in a team | 01 |

---

## How to practise (any level)

1. Read the diagram in the topic.
2. Explain the concept in your own words (out loud).
3. Answer the sample questions without looking.
4. Type a small example from memory.
5. Convert real JS you already wrote to TS — far better than toy examples.

---

## Rapid-fire answers

| Question | Short answer |
|---|---|
| Why TypeScript? | Catches errors at compile time; better autocomplete and refactoring. |
| Is TS a different language? | Superset of JS; compiles to JS; types are erased. |
| `any` vs `unknown`? | `any` disables checks; `unknown` forces narrowing first. |
| `interface` vs `type`? | Interfaces extend/merge; types handle unions and more. Both fine for objects. |
| `enum` vs union literal? | Union literals are erased and simpler; many teams prefer them. |
| What is a discriminated union? | Union with a shared literal field used to narrow. |
| `Pick` vs `Omit`? | Keep listed keys vs remove listed keys. |
| Why generic over `any`? | Keeps the input/output type relationship. |
| Type `useState(null)` initial user? | `useState<User \| null>(null)` |
| Type an input `onChange`? | `React.ChangeEvent<HTMLInputElement>` |
| Type a DOM ref? | `useRef<HTMLDivElement>(null)` |

---

## One useful closing style

> “I let TypeScript infer where it can and annotate at boundaries — props, function parameters, and API data. I avoid `any`, use `unknown` plus narrowing for untrusted values, and model states as discriminated unions so every case is handled.”

Adapt it to the actual question.

---

## Reminder

Questions in this repo are **samples for practice**.  
Real interviews vary by company, team, and year.  
Strong fundamentals + clear explanation matter more than memorising a list.
