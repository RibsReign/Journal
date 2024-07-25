# Day 29 (22.07.2024)

sdfsdfd

## Test

**Inputwithgets**  

```RUBY
irb :001 > name = gets
Bob
=> "Bob\n"
```

**Input with gets.chomp**  

```RUBY
irb :001 > name = gets.chomp
Bob
=> "Bob"
```

**Variable scope and block example**  

```RUBY
a = 5             # variable is initialized in the outer scope
3.times do |n|    # method invocation with a block, 'n' is the block parameter
  a = 3           # 'a' is accessible here and is being reassigned
end
puts a
```

**Duplication example**  

```RUBY
desired_location = "Barcelona"
johns_location = desired_location.dup

desired_location  # => "Barcelona"
johns_location    # => "Barcelona"
```

**Conditional example**  

```RUBY
if attack_by_land == true
  puts "release the goat"
elsif attack_by_sea == true
  puts "release the shark"
else
  puts "release Kevin the octopus"
end
```

**One-line if statement**  

```RUBY
puts "Hot diggity damn, 1 is less than 2" if 1 < 2
```

**Spaceship operator**  

```RUBY
5 <=> 10    #=> -1
10 <=> 10   #=> 0
10 <=> 5    #=> 1
```

**Case statement with variable assignment**  

```RUBY
grade = 'F'

did_i_pass = case grade #=> create a variable `did_i_pass` and assign the result of a call to case with the variable grade passed in
  when 'A' then "Hell yeah!"
  when 'D' then "Don't tell your mother."
  else "'YOU SHALL NOT PASS!' -Gandalf"
end
```

**Case statement with actions**  

```RUBY
grade = 'F'

case grade
when 'A'
  puts "You're a genius"
  future_bank_account_balance = 5_000_000
when 'D'
  puts "Better luck next time"
  can_i_retire_soon = false
else
  puts "'YOU SHALL NOT PASS!' -Gandalf"
  fml = true
end
```

**Unless statement**  

```RUBY
age = 19
unless age < 18
  puts "Get a job."
end
```

**Infinite loop with break**  

```RUBY
i = 0
loop do
  puts "i is #{i}"
  i += 1
  break if i == 10
end
```

**Until loop**  

```RUBY
i = 0
until i >= 10 do
 puts "i is #{i}"
 i += 1
end
```

**Inclusive and exclusive ranges**  

```RUBY
(1..5)      # inclusive range: 1, 2, 3, 4, 5
(1...5)     # exclusive range: 1, 2, 3, 4

# Ranges of letters
('a'..'d')  # a, b, c, d
```

**For loop**  

```RUBY
for i in 0..5
  puts "#{i} zombies incoming!"
end
```

**Upto and Downto methods**  

```RUBY
5.upto(10) { |num| print "#{num} " }     #=> 5 6 7 8 9 10
10.downto(5) { |num| print "#{num} " }   #=> 10 9 8 7 6 5
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
