# Day 42 (10.10.2024)

## REFLECTION

## NOTES

# Ruby Enumerable Methods Summary

## `include?`

- **Purpose**: Checks if a specific element is present in a collection.
- **Returns**: `true` if the element is found; otherwise, `false`.
- **Example**: `[1, 2, 3].include?(2)` returns `true`.

## `any?`

- **Purpose**: Checks if at least **one** element satisfies a given condition.
- **Returns**: `true` if at least one element meets the condition; otherwise, `false`.
- **Example**: `[1, 2, 3].any? { |num| num.even? }` returns `true`.

## `all?`

- **Purpose**: Checks if **all** elements satisfy a given condition.
- **Returns**: `true` if all elements meet the condition; otherwise, `false`.
- **Example**: `[1, 2, 3].all? { |num| num > 0 }` returns `true`.

## `none?`

- **Purpose**: Checks if **no** elements satisfy a given condition.
- **Returns**: `true` if no elements meet the condition; otherwise, `false`.
- **Example**: `[1, 2, 3].none? { |num| num > 3 }` returns `true`.

## `one?`

- **Purpose**: Checks if exactly **one** element satisfies a given condition.
- **Returns**: `true` if exactly one element meets the condition; otherwise, `false`.
- **Example**: `[1, 2, 3].one? { |num| num.even? }` returns `true`.

## PREVIOUS TASKS  

1. ~~Get a refresher~~  
2. ~~Continue learning about Ruby~~  
3. ~~Make sure to push Journal entries on time~~  

## REPEAT TASKS  

1. Meditation  
2. Flexbox Zombies  
3. Exercism  

