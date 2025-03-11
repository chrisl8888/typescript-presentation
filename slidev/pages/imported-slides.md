---
# Learning Objectives

- Understand the benefits of TypeScript over JavaScript
- Set up a TypeScript project with Jest for TDD
- Write basic TypeScript with type annotations

---
# Why TypeScript?

- Statically typed superset of JavaScript
- Helps catch errors at compile time
- Improves code maintainability and readability
- Provides better IDE support with autocompletion and type hints

---
# Setting Up a TypeScript Project

1. Install TypeScript globally:
   ```sh
   npm install -g typescript
   ```
2. Initialize a new TypeScript project:
   ```sh
   tsc --init
   ```
3. Install Jest and TypeScript support:
   ```sh
   npm install --save-dev jest ts-jest @types/jest
   ```
4. Configure Jest in `jest.config.js`:
   ```js
   module.exports = {
     preset: 'ts-jest',
     testEnvironment: 'node',
   };
   ```

---
# Writing Basic TypeScript

### Variable Annotations
```ts
let message: string = "Hello, TypeScript!";
console.log(message);
```

### Function Annotations
```ts
function add(a: number, b: number): number {
  return a + b;
}
```

### Interface Example
```ts
interface Person {
  name: string;
  age: number;
}

const user: Person = { name: "Alice", age: 25 };
console.log(user.name);
```

---
# Summary

- TypeScript enhances JavaScript with static typing
- Setting up TypeScript with Jest enables Test-Driven Development
- Basic type annotations improve code clarity and reliability
