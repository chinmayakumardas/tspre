# TS Atlas (tspre)

**Goal**  
One structured place to learn TypeScript the way interviews actually test it — basic types, reading type errors, modeling data, narrowing, utility types, and typing React / Next.js code.

*Interview-ready scope, not mastery.* Most 2 YOE interviews test TypeScript lightly: correct basic types, reading a type error, "why use TS at all", and typing a component's props. Advanced type-level programming (conditional types, mapped types, `infer`) is intentionally left out.

No playground. No external dependency required to understand the concepts.  
Diagrams first. Real usage. Sample interview questions (as thinking practice, not guarantees).

---

## Who this is for

| Experience | How to use this repo |
|---|---|
| **Fresher / 0–1 year** | Follow 01 → 06 in order. Focus on diagrams + basic examples. |
| **1–3 years** | Spend most time on 07–11. Practice interview questions out loud. |
| **3–6 years** | Skim 01–06, deepen 07–09, add trade-off answers (`interface` vs `type`, `enum` vs union). |

You should not need another resource to understand the **concepts** covered here.  
Official docs links (when present) are only for extra verification or latest details.

---

## How to use

1. Read the **diagram first** in every topic.
2. Read “Where it is used” — connects theory to real work.
3. Study examples and common mistakes.
4. Practice the sample interview questions out loud.
5. Do the matching challenge, then come back as a reference any time.

```text
Learning path
─────────────
01–04   Why TS + core types          ← Phase 1
05–06   Objects + functions          ← Phase 2
07–09   Unions, utility, generics    ← Phase 3 (highest yield)
10–11   React + Next.js              ← Phase 4 (highest yield)
12      Reading type errors
        Interview practice           ← Phase 5
```

---

## Topics

### Phase 1 — Why TypeScript & core types
| # | Topic | Master this |
|---|---|---|
| 01 | [Why TypeScript](./01-why-typescript/README.md) | The problem it solves, superset, erased types |
| 02 | [Basic types & inference](./02-basic-types-and-inference/README.md) | Primitives, arrays, tuples, annotations |
| 03 | [any vs unknown](./03-any-vs-unknown/README.md) | Why `any` defeats TS, `unknown` is safe |
| 04 | [Literal types & enums](./04-literal-types-and-enums/README.md) | Exact values, enum vs union |

### Phase 2 — Objects, interfaces & functions
| # | Topic | Master this |
|---|---|---|
| 05 | [Objects & interfaces](./05-objects-and-interfaces/README.md) | interface vs type, optional, readonly, index signatures |
| 06 | [Functions](./06-functions/README.md) | Param + return types, optional/default params |

### Phase 3 — Unions, narrowing & utility types
| # | Topic | Master this |
|---|---|---|
| 07 | [Unions & narrowing](./07-unions-and-narrowing/README.md) | Discriminated unions + type guards |
| 08 | [Utility types](./08-utility-types/README.md) | Partial, Required, Pick, Omit, Record |
| 09 | [Generics](./09-generics/README.md) | `<T>` placeholders, typed `groupBy` |

### Phase 4 — TypeScript with React & Next.js
| # | Topic | Master this |
|---|---|---|
| 10 | [TypeScript with React](./10-typescript-with-react/README.md) | Props, state, events, refs, hooks |
| 11 | [TypeScript with Next.js](./11-typescript-with-nextjs/README.md) | `params`, `searchParams`, Route Handlers |

### Phase 5 — Interview-specific practice
| # | Topic | Master this |
|---|---|---|
| 12 | [Reading type errors](./12-reading-type-errors/README.md) | Explain a TS error from a broken snippet |

### Extra
- [Interview preparation](./interview-preparation/README.md) — strategy and rapid-fire answers
- [Real-world examples](./real-world-examples/README.md)
- [Challenges](./challenges/README.md) — end-of-phase mini exercises
- [Tools & resources](./tools-and-resources/README.md)

---

## Interview questions note

Interview questions in this repo are **samples and thinking hints**.  
They are not a guarantee of what any company will ask.  
Technology and interview styles change. Use them to practice explaining concepts clearly.

---

## Design principles of this repo

- Diagram first (decision + flow)
- “Where it is used” in real applications
- Interview-ready scope — advanced type-level programming intentionally left out
- TypeScript-first examples
- Common mistakes shown as ❌ → ✅
- Self-contained explanations (no required external reading)

---

**Start here → [01. Why TypeScript](./01-why-typescript/README.md)**

Status: Active notes — structured and usable. Improving over time.
