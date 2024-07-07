# Day 18 (04.07.2024)

## A cheat sheet of array methods

### To add/remove elements

**push(...items)** – adds items to the end,
**pop()** – extracts an item from the end,
**shift()** – extracts an item from the beginning,
**unshift(...items)** – adds items to the beginning.
**splice(pos, deleteCount, ...items)** – at index pos deletes deleteCount elements and inserts items.
**slice(start, end)** – creates a new array, copies elements from index start till end (not inclusive) into it.
**concat(...items)** – returns a new array: copies all members of the current one and adds items to it. If any of items is an array, then its elements are taken.

### To search among elements

**indexOf/lastIndexOf(item, pos)** – look for item starting from position pos, and return the index or -1 if not found.
**includes(value)** – returns true if the array has value, otherwise false.
**find/filter(func)** – filter elements through the function, return first/all values that make it return true.
**findIndex** is like find, but returns the index instead of a value.

### To iterate over elements

**forEach(func)** – calls func for every element, does not return anything.

### To transform the array

**map(func)** – creates a new array from results of calling func for every element.
**sort(func)** – sorts the array in-place, then returns it.
**reverse()** – reverses the array in-place, then returns it.
**split/join** – convert a string to array and back.
**reduce/reduceRight(func, initial)** – calculate a single value over the array by calling func for each element and passing an intermediate result between the calls.

## Additionally

Array.isArray(value) checks value for being an array, if so returns true, otherwise false.

```JS
["Bilbo", "Gandalf", "Nazgul"].forEach((item, index, array) => {
  alert(`${item} is at index ${index} in ${array}`);
});
```

arr.**indexOf**(item, from) – looks for item starting from index from, and returns the index where it was found, otherwise -1.
arr.**includes**(item, from) – looks for item starting from index from, returns true if found.
The method arr.lastIndexOf is the same as indexOf, but looks for from right to left.

```JS
let arr = [1, 0, false];

alert( arr.indexOf(0) ); // 1
alert( arr.indexOf(false) ); // 2
alert( arr.indexOf(null) ); // -1

alert( arr.includes(1) ); // true
```

The **find** method looks for a single (first) element that makes the function return true.
If there may be many, we can use arr.filter(fn).
The syntax is similar to **find**, but filter returns an array of all matching elements:

```JS
let results = arr.filter(function(item, index, array) {
  // if true item is pushed to results and the iteration continues
  // returns empty array if nothing found
});

//For instance:

let users = [
  {id: 1, name: "John"},
  {id: 2, name: "Pete"},
  {id: 3, name: "Mary"}
];

// returns array of the first two users
let someUsers = users.filter(item => item.id < 3);

alert(someUsers.length); // 2
```

**reverse**  
The method arr.reverse reverses the order of elements in arr.
For instance:

```JS
let arr = [1, 2, 3, 4, 5];
arr.reverse();

alert( arr ); // 5,4,3,2,1
```

The call arr.**join**(glue) does the reverse to split. It creates a string of arr items joined by glue between them.

```JS
For instance:

let arr = ['Bilbo', 'Gandalf', 'Nazgul'];

let str = arr.join(';'); // glue the array into a string using ;

alert( str ); // Bilbo;Gandalf;Nazgul
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
