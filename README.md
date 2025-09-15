# TypeScript-Generics
Bunch of exercises for practicing TypeScript generics
Create a generic factory function which has type parameter and returns an instance of this type.
<details>
<summary>Hint</summary>
</details>
<details>
<summary>Solution</summary>
  
```typescript
  createInstance<T>(c: {new (): T}): T {
    return new c();
  }
```
</details>
