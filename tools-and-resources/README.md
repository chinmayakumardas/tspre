# Tools and Resources

Versions are intentionally not listed; check each tool's site.

## Official
| Resource | Link |
|---|---|
| TypeScript handbook | https://www.typescriptlang.org/docs/ |
| TypeScript Playground | https://www.typescriptlang.org/play |
| Utility types reference | https://www.typescriptlang.org/docs/handbook/utility-types.html |
| React + TypeScript docs | https://react.dev/learn/typescript |
| Next.js TypeScript docs | https://nextjs.org/docs/app/api-reference/config/typescript |
| MDN Web Docs | https://developer.mozilla.org |

## Build and quality
| Tool | Use |
|---|---|
| `tsc --noEmit` | Type-check without producing files |
| Vite / Next.js | Strip types and bundle |
| `typescript-eslint` | Lint rules (e.g. no `any`) |
| Prettier | Formatting |
| `tsx` | Run `.ts` files directly in Node |

## Ecosystem
| Need | Common choices |
|---|---|
| Runtime validation + types | Zod (`z.infer`), Valibot |
| Typed API data | OpenAPI generators, tRPC |
| Third-party types | `@types/*` packages (DefinitelyTyped) |
| Server data | TanStack Query, SWR |
| Forms | React Hook Form + Zod |

## Starter tsconfig
```json
{
  "compilerOptions": {
    "strict": true,
    "target": "ES2020",
    "module": "ESNext",
    "moduleResolution": "Bundler",
    "jsx": "preserve",
    "noEmit": true,
    "skipLibCheck": true
  }
}
```
`strict: true` turns on `strictNullChecks`, `noImplicitAny`, and related checks — keep it on.
