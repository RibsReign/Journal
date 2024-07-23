
# Day 28 (18.07.2024)

**capitalize**  

```RUBY
"hello".capitalize #=> "Hello"
```

**include?**  

```RUBY
"hello".include?("lo")  #=> true
"hello".include?("z")   #=> false
```

**upcase**  

```RUBY
"hello".upcase  #=> "HELLO"
```

**downcase**  

```RUBY
"Hello".downcase  #=> "hello"
```

**empty?**  

```RUBY
"hello".empty?  #=> false
"".empty?       #=> true
```

**length**  

```RUBY
"hello".length  #=> 5
```

**reverse**  

```RUBY
"hello".reverse  #=> "olleh"
```

**split**  

```RUBY
"hello world".split  #=> ["hello", "world"]
"hello".split("")    #=> ["h", "e", "l", "l", "o"]
```

**strip**  

```RUBY
" hello, world   ".strip  #=> "hello, world"
```

**sub and gsub**  

```RUBY
"he77o".sub("7", "l")           #=> "hel7o"
"he77o".gsub("7", "l")          #=> "hello"
```

**insert**  

```RUBY
"hello".insert(-1, " dude")     #=> "hello dude"
```

**delete**  

```RUBY
"hello world".delete("l")       #=> "heo word"
```

**prepend**  

```RUBY
"!".prepend("hello, ", "world") #=> "hello, world!"
```

**Converting other objects to strings**  
Using the to_s method, you can convert pretty much anything to a string. Here are some examples:

```RUBY
5.to_s        #=> "5"
nil.to_s      #=> ""
:symbol.to_s  #=> "symbol"
```

**Create a symbol**  
To create a symbol, put a colon at the beginning of some text:

```RUBY
:my_symbol
```

Symbols are stored in memory only once, making them faster in certain situations.

```RUBY
"string" == "string"  #=> true
"string".object_id == "string".object_id  #=> false
:symbol.object_id == :symbol.object_id    #=> true
```

It is possible to check if something is a nil type by using .nil?. For example:

```RUBY
irb :001 > "Hello, World".nil?
=> false

irb :001 > false == nil
=> false
```

While both false and nil are treated as negative when evaluated in an expression, they are not equivalent, as demonstrated by the above.

**puts vs return**  

```RUBY
a = puts "stuff"
puts a
```

What should we expect? a is assigned to the value returned by puts "stuff", which is nil. Therefore, puts a is the same as puts nil, which prints out an empty string. We are going to go much farther into puts and return later when we talk about methods, but we had to show you puts because we are going to be using it in future examples.

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
