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
  
```typescript
  function createArray<T = number>(amount: number): T[] {
    return new Array<T>(amount);
  }
```
</details>
