## How do Generics allow you to build reusable components and functions that stay strictly typed regardless of the data structures passed in?

Generics in TypeScript allow us to create reusable and strongly typed functions or components that work with different data types while still maintaining type safety.

Instead of writing separate functions for different types, we can use generics to make one flexible function.

Example:
function identity<T>(value: T): T {
  return value;
}

console.log(identity<string>("Hello"));
console.log(identity<number>(10));
