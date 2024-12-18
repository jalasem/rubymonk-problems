# Palindromes

## Problem Statement

Given a sentence, return true if the sentence is a palindrome.

You are supposed to write a method palindrome? to accomplish this task.

Note Ignore whitespace and cases of characters.

##Example:

Given "Never odd or even" the method should return true

## Solution

```ruby
def palindrome?(sentence)
  clean_sentence = sentence.gsub(/[^a-z0-9]/i, '').downcase
  
  clean_sentence == clean_sentence.reverse
end
```