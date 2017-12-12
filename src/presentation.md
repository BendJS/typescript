class: center, middle
name: introduction

# Getting Started with Typescript

## BendJS 2017.12.12
---

class: center, middle
name: introduction
# Adam Horak

## Solution Architect @
.column.is-half.is-offset-one-quarter[![Frontline](/img/frontline.png)]
---

# What is Typescript

* Superset of JavaScript with static typing
* Includes some future JS features (dynamic import, decorators, etc)
* Compiles to plain JavaScript (configurable targets based on ES5, ES6, etc)
* Plain old JavaScript is valid TypeScript!
---

# Why

* Catches code that is not type safe before it is run and eliminates some hidden bugs
* Communicates type information that could otherwise be implicit to other developers
* Reminds future me of WTF I was thinking when I wrote something 6 months ago
* Imposes discipline in design
* Refactoring!
---

# Why Not?

* Extra friction for setup and compilation
* Unnecessary overhead for prototyping or small projects
* More syntax to learn and concepts to understand
---

# Setting up a TypeScript project

* `echo "{}" >> tsconfig.json && touch index.ts`
* done!
---

# Basic type annotations and type inference

```typescript 
const foo: string = “foo”;
const sayHello = (name: string): string => `Hello ${name}`
const sayHello = function(name: string): string {...} 
```

* Basic Types:
    * boolean
    * number
    * string
    * array
    * tuple
    * null
    * undefined
* Inline type annotations
---

# Interfaces

* Define object shapes and member types
* Define function parameters + return types
* Optional properties
* Readonly properties
* Index signatures
* Extending interfaces
---

# Type aliases

* “type” keyword declares a type that can be re-used elsewhere
* You can declare a type alias with any type annotation
---

# Union and intersection types

* Union types declare an “or” relationship
* Intersection types declare and “and” relationship
---

# Escape hatches

* Any type
* Type assertions
---

# Generics
* Type variables
* `function identity<T> (arg: T): T { return arg; }`
* Often inferred
* Generic constraints
* Examples:
    * `Promise<number>`
    * `Array<string>`
---

# Enums

* Numeric enums
* String enums
* Run-time code
---

# Configuring compilation behavior

* `tsconfig.json`
* `noImplicitAny`
* `strictNullChecks`
---

# Third party libraries

* DefinitelyTyped
* `npm install @types/express`
---

# A (very) simple example

* Type safe Express API
---



