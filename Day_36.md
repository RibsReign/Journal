# Day 36 (03.08.2024)

Had to take a break eventually because I ran out of hours for codespaces. Also went irl stuff, sigh oh well back at it.
Today I did enumerable exercises progress is slow right now.

**Selecting and Rejecting Elements**  

```ruby
friends = ['Sharon', 'Leo', 'Leila', 'Brian', 'Arun']

friends.select { |friend| friend != 'Brian' }
 #=> ["Sharon", "Leo", "Leila", "Arun"]

friends = ['Sharon', 'Leo', 'Leila', 'Brian', 'Arun']

friends.reject { |friend| friend == 'Brian' }
 #=> ["Sharon", "Leo", "Leila", "Arun"]
```

**Using each Method**  

```ruby
friends = ['Sharon', 'Leo', 'Leila', 'Brian', 'Arun']

friends.each { |friend| puts "Hello, " + friend }

# => Hello, Sharon
# => Hello, Leo
# => Hello, Leila
# => Hello, Brian
# => Hello, Arun

# => ["Sharon", "Leo", "Leila", "Brian" "Arun"]

my_array = [1, 2]

my_array.each do |num|
  num *= 2
  puts "The new number is #{num}."
end

# => The new number is 2.
# => The new number is 4.

# => [1, 2]
```

**each with Hashes**  

```ruby
my_hash = { "one" => 1, "two" => 2 }

my_hash.each { |key, value| puts "#{key} is #{value}" }

one is 1
two is 2
# => { "one" => 1, "two" => 2}

my_hash.each { |pair| puts "the pair is #{pair}" }

the pair is ["one", 1]
the pair is ["two", 2]
# => { "one" => 1, "two" => 2}
```

**The each_with_index Method**  

```ruby
fruits = ["apple", "banana", "strawberry", "pineapple"]

fruits.each_with_index { |fruit, index| puts fruit if index.even? }

# => apple
# => strawberry
# => ["apple", "banana", "strawberry", "pineapple"]
```

**Using map Method**  

```ruby
friends = ['Sharon', 'Leo', 'Leila', 'Brian', 'Arun']

friends.map { |friend| friend.upcase }
# => `['SHARON', 'LEO', 'LEILA', 'BRIAN', 'ARUN']`

my_order = ['medium Big Mac', 'medium fries', 'medium milkshake']

my_order.map { |item| item.gsub('medium', 'extra large') }
# => ["extra large Big Mac", "extra large fries", "extra large milkshake"]
```

**Using select with Hashes**  

```ruby
responses = { 'Sharon' => 'yes', 'Leo' => 'no', 'Leila' => 'no', 'Arun' => 'yes' }
responses.select { |person, response| response == 'yes'}
# => {"Sharon"=>"yes", "Arun"=>"yes"}
```

**Using reduce Method**  

```ruby
my_numbers = [5, 6, 7, 8]

my_numbers.reduce { |sum, number| sum + number }
# => 26

my_numbers = [5, 6, 7, 8]

my_numbers.reduce(1000) { |sum, number| sum + number }
# => 1026

votes = ["Bob's Dirty Burger Shack", "St. Mark's Bistro", "Bob's Dirty Burger Shack"]

votes.reduce(Hash.new(0)) do |result, vote|
  result[vote] += 1
  result
end
# => {"Bob's Dirty Burger Shack"=>2, "St. Mark's Bistro"=>1}
```

**Hash with Default Value**  

```ruby
hundreds = Hash.new(100)
hundreds["first"]         #=> 100
hundreds["mine"]          #=> 100
hundreds["yours"]         #=> 100
```

## PREVIOUS TASKS

1. Continue learning about Ruby
2. Make sure to push Journal entries on time.

## REPEAT TASKS

1. Meditation
2. Flexbox Zombies
3. Exercism
4. LeetCode

## TODO

1. ~~Continue learning about Ruby~~
2. ~~Make sure to push Journal entries on time.~~

## REFLECTION
