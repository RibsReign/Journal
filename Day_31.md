# Day 31 (24.07.2024)

**Flattening Nested Arrays**  

```ruby
irb: 001 > a = [1, 2, [3, 4, 5], [6, 7]]
=> [1, 2, [3, 4, 5], [6, 7]]
irb: 002 > a.flatten
=> [1, 2, 3, 4, 5, 6, 7]
```

**Using each Method**  

```ruby
irb :003 > a = [1, 2, 3]
irb :004 > a.each { |e| puts e + 2 }
3
4
5
=> [1, 2, 3]
```

**Using map Method**  

```ruby
irb :011 > a = [1, 2, 3]
irb :012 > a.map { |x| x**2 }
=> [1, 4, 9]
```

**Using uniq! Method**  

```ruby
irb :013 > b = [1, 1, 2, 2, 3, 3, 4, 4]
=> [1, 1, 2, 2, 3, 3, 4, 4]
irb :014 > b.uniq!
=> [1, 2, 3, 4]
irb :015 > b
=> [1, 2, 3, 4]
```

## PREVIOUS TASKS

1. ~~Continue learning about Ruby~~
2. Make sure to push Journal entries on time.

## REPEAT TASKS

1. Meditation
2. Flexbox Zombies
3. LeetCode

## TODO

1. Continue learning about Ruby
2. Make sure to push Journal entries on time.

## REFLECTION
