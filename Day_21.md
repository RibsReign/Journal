# Day 21 (07.07.2024)

I've come to learn that once again reading is KEY and I should always doublecheck what I actually need to make or I end up confusing myself and making needless mistakes.
I've learned about sets.
In JavaScript, a **Set** is a built-in object that allows you to store unique values of any type, whether primitive values or object references.

```JS
let set = new Set();

set.add(1); // Adding elements to Set
set.add(2);
set.add(3);
set.add(1); // Duplicate value, won't be added

console.log(set); // Output: Set { 1, 2, 3 }

console.log(set.size); // Size of the Set: 3

set.delete(2); // Deleting an element from Set
console.log(set); // Output: Set { 1, 3 }

console.log(set.has(1)); // Checking if Set has value: true
console.log(set.has(2)); // Checking if Set has value: false

set.forEach(value => {
  console.log(value); // Iterating over Set elements
});
```

## PREVIOUS TASKS

1. ~~Continue or Finish object Basics~~

## REPEAT TASKS

1. Meditation
2. Flexbox Zombies
3. LeetCode

## TODO

1. Continue or Finish object Basics

## REFLECTION

Read, Read and once again read what you are actually supposed to do.
