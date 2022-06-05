# Loose equals

Explicit (and silly-joky 🤡) non-strict equality comparator.

JavaScript has a strict comparison operator (`===`) and a loose comparison operator (`==`). Best practice is to use strict comparison. However, sometimes you need to [loosely compare](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness#Loose_equality_using) some values.

You better be explicit about using loose comparison. Comments are not reliable since they get out of date very quickly. The most efficient and explicit way to say something in code is to say something _with the code_.

## Installation

```
npm i loose-equals
```

## Usage

```js
import { looseEquals } from "loose-equals";

1 === 1; // true
1 === "1"; // false

looseEquals(1, 1); // true
looseEquals("1", 1); // true
```
