## TypeScript Tutorial

A small, self‑contained codebase for learning modern TypeScript by reading and running focused examples.  
Each file in `src` introduces one core language feature, building up from the basics to more advanced patterns and best practices.

---

### Prerequisites

- **Node.js**: v16+ recommended  
- **npm**: comes with Node  
- **TypeScript**: already listed as a dev dependency in this project

---

### Getting Started

1. **Install dependencies**

   ```bash
   npm install
   ```

2. **Open the project in your editor**

   Open the folder `typescript-practices` in VS Code or your preferred IDE with TypeScript support.

---

### How to Run the Examples

This repository is designed for you to run individual `.ts` files and inspect their output.

- **Option 1 – Compile with `tsc` and run with Node**

  ```bash
  # Compile a single file to JavaScript
  npx tsc src/01-basics.ts --outDir dist

  # Execute the compiled JavaScript
  node dist/01-basics.js
  ```

  You can replace `01-basics.ts` with any other file in `src`.

- **Option 2 – Use `ts-node` (optional)**

  If you prefer running TypeScript directly without a manual compile step:

  ```bash
  npm install --save-dev ts-node

  npx ts-node src/01-basics.ts
  ```

---

### Project Structure

All learning material lives in the `src` folder:

- `01-basics.ts` – **Basic TypeScript syntax** and minimal example setup
- `02-basic-types.ts` – **Primitive types**, arrays, tuples, and other core types
- `03-type-inference.ts` – **Type inference rules** and how TypeScript infers types for you
- `04-functions.ts` – **Functions**, parameters, default values, optional params, and return types
- `05-objects-interfaces.ts` – **Objects and interfaces**, structural typing, and interface extension
- `06-type-aliases.ts` – **Type aliases** for primitives, unions, objects, and function types
- `07-union-intersection.ts` – **Union and intersection types**, modeling flexible data shapes
- `08-literal-types.ts` – **Literal types** and narrowing with specific string/number values
- `09-type-assertions-guards.ts` – **Type assertions** and **type guards** for safe runtime checks
- `10-classes.ts` – **Classes**, access modifiers, inheritance, and basic OOP patterns
- `11-generics.ts` – **Generics** for reusable, type‑safe functions, classes, and interfaces
- `12-utility-types.ts` – Built‑in **utility types** like `Partial`, `Pick`, `Readonly`, etc.
- `13-enums.ts` – **Enums** and how to model sets of named constants
- `14-async-await.ts` – **Async/await**, promises, and typed asynchronous code
- `15-best-practices.ts` – **Best practices** for real‑world TypeScript projects
- `example-api-client/` – A small **API client example** showing how to type HTTP calls
  - `example-api-client/types.ts` – Shared types and interfaces for API data
  - `example-api-client/api.ts` – Example of a typed API client using those types

---

### Recommended Learning Path

1. **Read the file** from top to bottom, paying attention to type annotations and comments.  
2. **Run the file** (using `tsc` or `ts-node`) and observe the output or any compile‑time errors.  
3. **Experiment**:
   - Change types and see how the compiler reacts.
   - Introduce intentional mistakes to learn from error messages.
   - Add your own examples below the existing ones.

Move in numerical order (`01` → `15`), and then explore the `example-api-client` folder as a more realistic mini‑project.

---

### Customizing the Setup

- **Compiler options**: You can create a `tsconfig.json` file to control target, module system, strictness, and more.  
- **Scripts**: You can add `npm` scripts (e.g. `"dev": "ts-node src/01-basics.ts"`) to automate running examples.

These are optional and not required to understand the tutorial code itself.

---
