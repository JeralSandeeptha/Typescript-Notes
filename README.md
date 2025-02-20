# Typescript Notes

---

## Table of Content
- [Installation](#installation)
- [Run File](#run-file)
- [Types](#types)
- [Primitive Types](#primitive-types)
- [Functions](#functions)

---

## Installation

Global Installation
```bash
npm i -g typescript
```

Local Installation
```bash
npm i typescript --save-dev
```

Check version
```bash
tsc -v
```

## Run File

Basically we can compile the .ts file. It will create a .js file.
```js
tsc index.js
```

---

## Types

- Number
- String
- Boolean
- Null
- Undefined
- Void
- Object
- Array
- Tupple
- Any
- Never

etc.

---

## Primitive Types

```js
const name: string = 'Jeral Sandeeptha';

const count: number = 55;

const isTrue: boolean = false;
```

---

## Functions

Simple Parameters
```js
function addNumbers(num: number) {
    return num + 2;
}

addNumbers(4);
```

Multiple Parameters
```js
function signUp(name: string, email: string, password: string, isVerified: boolean) {
    console.log('User registered');
}

signUp('Jeral Sandeeptha', 'jeral.sandeeptha1@gmail.com', 'mnjs0529', false); 
```

Default values
```js
function signUp(name: string, email: string, password: string, isVerified: boolean = false) {
    console.log('User registered');
}

signUp('Jeral Sandeeptha', 'jeral.sandeeptha1@gmail.com', 'mnjs0529', false); 
```

With return values
```js
function addNumbers(num: number): number {
    return num + 2;
}

addNumbers(4);
```
```js
const heros: string[] = [];

heros.map((hero: string): string => {
    return `Hero is ${hero}`;
});
```

With multiple return data types
```js

```

functions with Any data type. If we don't return values it mean void
```js
const consoleError = (error: string): void => {
    console.log(error);
}
```

functions with Never data type. This is used to forcefull termination of program
```js
const consoleError = (error: string): never => {
    throw new Error(error);
}
```