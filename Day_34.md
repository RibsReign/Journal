# Day  ()
**Debugging with Pry-byebug**  
To use Pry-byebug, you just need to call binding.pry at any point in your program.

require 'pry-byebug'

def isogram?(string)
  original_length = string.length
  string_array = string.downcase.split

  binding.pry

  unique_length = string_array.uniq.length
  original_length == unique_length
end

isogram?("Odin")

## PREVIOUS TASKS

1.
2.

## REPEAT TASKS

1. Meditation
2. Flexbox Zombies
3. LeetCode

## TODO

1. a
2. a

## REFLECTION