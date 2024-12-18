# Kaprekar's Number

## Problem Statement

9 is a Kaprekar number since
9 ^ 2 = 81 and 8 + 1 = 9

297 is also Kaprekar number since
297 ^ 2 = 88209 and 88 + 209 = 297.

In short, for a Kaprekar number k with n-digits, if you square it and add the right n digits to the left n or n-1 digits, the resultant sum is k.

Find if a given number is a Kaprekar number.

## Solution
```ruby
def kaprekar?(k)
  square_str = (k**2).to_s
  mid = square_str.length / 2
  left = square_str[0...mid]
  right = square_str[mid..-1]
  
  left = left.empty? ? 0 : left.to_i
  right = right.to_i
  
  k == left + right
end
```
