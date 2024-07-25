# Day 30 (23.07.2024)

**Array Creation and Initialization**  

```ruby
Array.new #=> []
Array.new(3) #=> [nil, nil, nil]
Array.new(3, 7) #=> [7, 7, 7]
Array.new(3, true) #=> [true, true, true]
```

**Accessing Array Elements**  

```ruby
str_array = ["This", "is", "a", "small", "array"]
str_array.first #=> "This"
str_array.first(2) #=> ["This", "is"]
str_array.last(2) #=> ["small", "array"]
```

**Adding and Removing Elements**  

```ruby
num_array = [1, 2]
num_array.push(3, 4) #=> [1, 2, 3, 4]
num_array << 5 #=> [1, 2, 3, 4, 5]
num_array.pop #=> 5
num_array #=> [1, 2, 3, 4]

num_array = [2, 3, 4]
num_array.unshift(1) #=> [1, 2, 3, 4]
num_array.shift #=> 1
num_array #=> [2, 3, 4]

num_array = [1, 2, 3, 4, 5, 6]
num_array.pop(3) #=> [4, 5, 6]
num_array.shift(2) #=> [1, 2]
num_array #=> [3]
```

**Array Operations**  

```ruby
[1, 1, 1, 2, 2, 3, 4] - [1, 4] #=> [2, 2, 3]
[].empty? #=> true
[[]].empty? #=> false
[1, 2].empty? #=> false
[1, 2, 3].length #=> 3
[1, 2, 3].reverse #=> [3, 2, 1]
[1, 2, 3].include?(3) #=> true
[1, 2, 3].include?("3") #=> false
[1, 2, 3].join #=> "123"
[1, 2, 3].join("-") #=> "1-2-3"
```

**Deleting Elements**  

```ruby
irb :005 > a.delete_at(1)
=> 2
irb :006 > a
=> [1, 3, 4]

irb :007 > my_pets = ["cat", "dog", "bird", "cat", "snake"]
=> ["cat", "dog", "bird", "cat", "snake"]
irb :008 > my_pets.delete("cat")
=> "cat"
irb :009 > my_pets
=> ["dog", "bird", "snake"]
```

**Removing Duplicates**  

```ruby
irb :010 > b = [1, 1, 2, 2, 3, 3, 4, 4]
=> [1, 1, 2, 2, 3, 3, 4, 4]
irb :011 > b.uniq
=> [1, 2, 3, 4]
irb :012 > b
=> [1, 1, 2, 2, 3, 3, 4, 4]
```

**Array Selection**  

```ruby
irb :001 > numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
=> [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
irb :002 > numbers.select { |number| number > 4 }
=> [5, 6, 7, 8, 9, 10]
irb :003 > numbers
=> [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

## PREVIOUS TASKS

1. ~~Continue learning about Ruby~~
2. ~~Make sure to push Journal entries on time.~~

## REPEAT TASKS

1. Meditation
2. Flexbox Zombies
3. LeetCode

## TODO

1. Continue learning about Ruby
2. Make sure to push Journal entries on time.

## REFLECTION

You can now copy this text and paste it directly into a .txt file. The markdown formatting will be preserved, and you can then use this file as needed.