# Typescript Course

## Glossary

- **Compile Time vs Runtime**: We consider the time before your code is executed to be “Compile Time”. Anything that happens in your program after you execute your code happens at runtime.
- **Dynamic Types vs Static Types**: Languages like Java and C++ expect variables to always be the same type after they are declared. They use static, or unchanging, types. Other languages, like JavaScript and Python, let you change the type of variables at runtime. These use dynamic types.
- **Type Error**: When the program throws an error because a value of one type was used when the program was expecting another type. This happens when we use numbers in place of strings or if we try to call a function, only to find out it is really undefined.
- **Type Safety**: Eliminating type errors by ensuring types are only used in the correct place. This usually happens by having a compiler warn you when you use a type in the wrong way. There are varying degrees of type safety, from incredibly rigid with a low chance of type errors to more flexible with a higher chance of type errors.
- **Static Analysis or Static Validation**: When a tool analyzes your code without executing it. This can give you some insights into ways to improve your code and can warn you of errors before you run your code.
- **Compiler**: A program which takes code and transforms it into another format. Typically compilers convert code into machine code which is run directly by the CPU, but other compilers, like TypeScript, convert from one programming language into another programming language.
- **Type Annotations:** Small bits of code that tell TypeScript what type a value or variable is.
- **Type Declaration**: A file with the .d.ts extension which only holds type definitions for a JavaScript library.

## JavaScript Types

### Primative types

- **Boolean** - True or false;
- **Number** - Stored as floats, the same type for whole integers and decimals. NaN (Not a Number).
- **BigInt** - introduced in ES2019, for very large integers. Created by adding a little n after the number literal. 1337n !== 1377
- **String** - Text data
- **Symbol** - Unique and imutable. You can pass in a desription but two Symbols with the same description will not be equal.
- **undefined** - it has no value. You will find this when you check a variable that does not exist yet.
- **null** lack of value. The variable is defined but has no value. let nullish = null; typeof nullish; //"object"; nullish === null; //true

### Structural Types

- **Object** - Object is the most versatile type in JavaScript. An Object can have any number of properties, each with its own value. This allows you to create unique and interesting data structures. Objects typically use Strings for indexing the properties, but Symbols can be used as well. A property’s value can be any type. Objects are compared by reference not value. 2 objects with the same values will not be equal. Comparing a clone of an object will be equal to the object.
- **Array** - typeOf will return Object even though they are not the same. Array.isArray(myArray) = true;
- **Function** - Functions are defined blocks of code that you can call from elsewhere in your program. They can take parameters and have a return value. One of the best things about JavaScript is that functions can be treated as values. That means you can pass them between functions or use them whenever you want. That means that Functions are their own type as well.
- **Classes** - Classes were introduced to JavaScript in ES2015 and serve as syntactic sugar around JavaScript’s prototypical inheritance system. We’ll talk more about classes later in the course, but for now we can look at the types that classes generate.
