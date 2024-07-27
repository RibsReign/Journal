# Day 32 (25.07.2024)

**Hash Creation and Basic Operations**  

```ruby
my_hash = {
  "a random word" => "ahoy",
  "Dorothy's math test score" => 94,
  "an array" => [1, 2, 3],
  "an empty hash within a hash" => {}
}

my_hash = Hash.new
my_hash               #=> {}

hash = { 9 => "nine", :six => 6 }

shoes = {
  "summer" => "sandals",
  "winter" => "boots"
}

shoes["summer"]   #=> "sandals"
shoes["hiking"]   #=> nil
shoes.fetch("hiking")   #=> KeyError: key not found: "hiking"

shoes["fall"] = "sneakers"
shoes     #=> {"summer"=>"sandals", "winter"=>"boots", "fall"=>"sneakers"}

shoes.delete("summer")    #=> "flip-flops"
shoes                     #=> {"winter"=>"boots", "fall"=>"sneakers"}
```

**Hash Methods**  

```ruby
books = {
  "Infinite Jest" => "David Foster Wallace",
  "Into the Wild" => "Jon Krakauer"
}

books.keys      #=> ["Infinite Jest", "Into the Wild"]
books.values    #=> ["David Foster Wallace", "Jon Krakauer"]

hash1 = { "a" => 100, "b" => 200 }
hash2 = { "b" => 254, "c" => 300 }
hash1.merge(hash2)      #=> { "a" => 100, "b" => 254, "c" => 300 }
```

**Iterating Over Hashes**  

```ruby
person = {name: 'bob', height: '6 ft', weight: '160 lbs', hair: 'brown'}

person.each do |key, value|
  puts "Bob's #{key} is #{value}"
end
```

**Hash Syntax Styles**  

```ruby
american_cars = {
  :chevrolet => "Corvette",
  :ford => "Mustang",
  :dodge => "Ram"
}

japanese_cars = {
  honda: "Accord",
  toyota: "Corolla",
  nissan: "Altima"
}

american_cars[:ford]    #=> "Mustang"
japanese_cars[:honda]   #=> "Accord"
```

**More Hash Methods**  

```ruby
name_and_age = { "Bob" => 42, "Steve" => 31, "Joe" => 19}
name_and_age.key?("Steve")  #=> true
name_and_age.key?("Larry")  #=> false

name_and_age.select { |k,v| k == "Bob" }  #=> {"Bob"=>42}
name_and_age.select { |k,v| (k == "Bob") || (v == 19) }  #=> {"Bob"=>42, "Joe"=>19}

name_and_age.fetch("Steve")  #=> 31
name_and_age.fetch("Larry", "Larry isn't in this hash")  #=> "Larry isn't in this hash"

name_and_age.to_a  #=> [["Bob", 42], ["Steve", 31], ["Joe", 19]]

name_and_age.keys  #=> ["Bob", "Steve", "Joe"]
name_and_age.values  #=> [42, 31, 19]
```

**Iterating Over Keys and Values**  

```ruby
opposites = {positive: "negative", up: "down", right: "left"}

opposites.each_key { |key| puts key }
opposites.each_value { |value| puts value }
opposites.each { |key, value| puts "The opposite of #{key} is #{value}" }
```

**Creating a Method**  

```ruby
def my_name
  "Joe Smith"
end

puts my_name    #=> "Joe Smith"

def greet(name = "stranger")
  "Hello, " + name + "!"
end

puts greet("Jane") #=> Hello, Jane!
puts greet #=> Hello, stranger!

def even_odd(number)
  unless number.is_a? Numeric
    return "A number was not entered."
  end

  if number % 2 == 0
    "That is an even number."
  else
    "That is an odd number."
  end
end

puts even_odd(20) #=>  That is an even number.
puts even_odd("Ruby") #=>  A number was not entered.
```

**Chaining Methods**  

```ruby
phrase = ["be", "to", "not", "or", "be", "to"]

puts phrase.reverse.join(" ").capitalize
# => "To be or not to be"
```

**Bang Methods**  

```ruby
puts whisper.downcase! #=> "hello everybody"
puts whisper #=> "hello everybody"
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
