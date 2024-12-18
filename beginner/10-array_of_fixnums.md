# Check if all elements in an array are Fixnum

## Problem Statement
Given an array, return true if all the elements are Fixnums.

You need to write array_of_fixnums? method to accomplish this task.

### Example:
Given [1,2,3], the method should return true

## Solution
```ruby
def array_of_fixnums?(array)
  array.all? { |n| n.is_a? Integer }
end
```