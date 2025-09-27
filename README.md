# TypeScript-Generics
Bunch of exercises for practicing TypeScript generics

## Function Generics
🔷  **Factory function**

***Task***

Create a generic factory function which has type parameter and returns an instance of this type.
<details>
<summary>💡Hint</summary>
</details>
<details>
<summary>✅ Solution</summary>
  
```ts
  function createInstance<T>(c: {new (): T}): T {
    return new c();
  }
```
</details>



🔷 **Generic Defaults**

***Task***

Create a generic functions with type parameter T which returns array of type T, but if no parameter passed return array of Number.
<details>
<summary>💡Hint</summary>

  Use parameter defaults
</details>
<details>
<summary>✅ Solution</summary>
</details>

## Conditional Generics

***Task***

Create a generic Type that takes a function type and returns its return type
<details>
<summary>💡Hint</summary>
  Check the type to extend the function type and use infer keyword
</details>
<details>
<summary>✅ Solution</summary>
  
```ts
type ReturnType1<T> = T extends (...args: any[])=> infer R ? R : never
```
</details>

