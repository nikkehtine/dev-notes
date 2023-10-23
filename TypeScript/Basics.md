# TypeScript Basics [📝](https://www.typescriptlang.org/docs/)

## Tooling [📝](https://www.typescriptlang.org/docs/handbook/typescript-tooling-in-5-minutes.html)

```bash
tsc <files>
```

- `--noImplicitAny`: raise errors on expressions and declarations with an implied `any` type
- `--noEmitOnError`: don't emit any files if type checking errors are reported
- `--target`: specify a target ECMAscript version

## Type annotations

```typescript
let sum: number = 1 + 1;
sum; // 2
```

```typescript
let b: boolean = true || false;
b; // true
```

```typescript
let b: boolean = 1 + 1;
b; // type error: Type 'number' is not assignable to type 'boolean'.
```
