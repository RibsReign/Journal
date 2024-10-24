# Day 43 (10.10.2024)

## Task: Delete Seat at Seat Index

To remove a seat at the `seat_index` of the row at `row_index` in the chart:

```ruby
chart[row_index].delete_at(seat_index)
chart
```

## Example of Using Filter Methods

### Filter Map for Arrays

The `filter_map` method creates arrays:

```ruby
vehicles.filter_map { |name, data| name if data[:year] >= 2020 }
```

Result:

```ruby
[:caleb, :dave]
```

### Using Compact to Remove Nil Values

The `compact` method removes `nil` values from an array:

```ruby
vehicles.collect { |name, data| name if data[:year] >= 2020 }.compact
```

Result:

```ruby
[:caleb, :dave]
```

Without `compact`:

```ruby
vehicles.collect { |name, data| name if data[:year] >= 2020 }
```

Result:

```ruby
[nil, :caleb, :dave]
```

### Select for Filtering Hashes

The `select` method is used to filter hashes:

```ruby
vehicles.select { |name, data| data[:year] >= 2020 }
```

Result:

```ruby
{:caleb=>{:year=>2020, :make=>"Honda", :model=>"Accord"}, :dave=>{:year=>2021, :make=>"Ford", :model=>"Escape"}}
```

## Modifying Hash Values

To delete the `:color` key from a specific vehicle (e.g., `:dave`):

```ruby
vehicles[:dave].delete(:color)
```

Result:

```ruby
"red"
```

The updated `vehicles` hash is:

```ruby
{:alice=>{:year=>2019, :make=>"Toyota", :model=>"Corolla"}, :caleb=>{:year=>2020, :make=>"Honda", :model=>"Accord"}, :dave=>{:year=>2021, :make=>"Ford", :model=>"Escape"}}
```

To access specific details:

```ruby
vehicles[:alice][:year] # => 2019
vehicles[:blake][:make] # => "Volkswagen"
vehicles[:caleb][:model] # => "Accord"
```

## Example: Iterating Over Flattened Arrays

Flatten and iterate over arrays:

```ruby
teacher_mailboxes.flatten.each do |teacher|
  puts "#{teacher} is amazing!"
end
```

Output:

```ruby
Adams is amazing
Baker is amazing
Clark is amazing
...
```

## TODO

1. Continue learning about Ruby.
2. Make sure to push journal entries on time.

## Repeat Tasks

1. Meditation
2. Flexbox Zombies
3. Exercism
4. LeetCode
