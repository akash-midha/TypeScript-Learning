# TypeScript

    - TypeScript is superset of JavaScript developed by Microsoft. Everything we can do in JS, it can be done in TS. (Ts is wrapper over JS)
    - All valid JavaScript is also valid TypeScript.
    - But TypeScript adds static type checking, interfaces, enums, and other features not present in vanilla JS.
    - It compiles (or transpiles) down to plain JavaScript that browsers can run. TS is developmemt tool as code is transpiled /copiled to JS.
    - It helps us to catch errors at the time of compilation and not runtime.

## 🔹 Why Use TypeScript?
- ✅ Type Safety (detects errors during compile time)
- ✅ Better IDE support (autocomplete, type inference)
- ✅ More maintainable and readable code
- ✅ Ideal for large codebases and teams

## Compile ts to js

```bash
tsc index.ts
```

## 🔹 Basic Types

```ts
let isDone: boolean = true;
let count: number = 10;
let username: string = "Akash";
let list: number[] = [1, 2, 3];
let tuple: [string, number] = ["hello", 5];
let anyValue: any = "Can be anything";
let nothing: void = undefined;
let value: unknown = "unknown value";
```

## 🔹 Functions

Never Type: never represents value which are never observed. In return type, this means that function throws an exception or terminates execution of program.

```ts
function add(a: number, b: number): number {
  return a + b;
}

function logMessage(msg: string): void {
  console.log(msg);
}

function handleError(error: string): never {
    throw new Error(error);
}
```
