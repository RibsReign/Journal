# Day 34 (27.07.2024)

I spend today reading learning how to learn pry and debugging why rbenv is not working.

**Debugging with Pry-byebug**  

To use Pry-byebug, you just need to call binding.pry at any point in your program. You can use the ls command to see what methods and instance variables an object has access to. If you don't want to use the require you can do this: ruby -rpry app.rb

```ruby
require 'pry-byebug'

def isogram?(string)
  original_length = string.length
  string_array = string.downcase.split

  binding.pry

  unique_length = string_array.uniq.length
  original_length == unique_length
end

isogram?("Odin")
```

## PREVIOUS TASKS

1. ~~Continue learning about Ruby~~
2. Make sure to push Journal entries on time.

## REPEAT TASKS

1. Meditation
2. Flexbox Zombies
3. Exercism
4. LeetCode

## TODO

1. Continue learning about Ruby
2. Make sure to push Journal entries on time.

## REFLECTION
