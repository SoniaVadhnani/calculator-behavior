# Addition

## Scenario: Addition of two positive numbers

Given - The calculator is ON.

When -  I type in "positive number"
And I press "plus"
And I type in "positive number"
And I press "equals"

Then - I see the "added number" as the result.

## Scenario: Addition of two negative numbers

Given - The calculator is ON.

When - I type in "negative number"
And I press "plus"
And I type in "negative number"
And I press "equals".
  
Then - I see the "added number" as the result which is also a negative number.

## Scenario: Addition of fractions

Given - The calculator is ON.

When - I type in "numerator followed by division sign followed by denominator"
And I press "plus"
And I type in "numerator followed by division sign followed by denominator"
And I press "equals".
  
Then - I see the "added number" as the result.

## Scenario: of positive and negative number
  
Given - The calculator is ON.

When - I type in "positive number"
And I press "plus"
And I type in "negative number"
And I press "equals".
  
Then - I see the "added number" as the result.

## Scenario: Addition of decimals

Given - The calculator is ON.

When - I type in "decimal number"
And I press "plus"
And I type in "decimal number"
And I press "equals".
  
Then - I see the "added number" as the result.

## Scenario: Typing operator more than once

Given - The calculator is ON.

When - I type in "positive or negative number"
And I press "plus"
And I type in "plus"
And I press "equals".
  
Then - The result is the same number given as input.

## Scenario: Addition of more than 2 numbers

Given - The calculator is ON.

When - I type any number
And I press "plus"
And I type in "positive number" or "negative number in braces"
And I press "plus"
And I type in "positive number" or "negative number in braces"
And I press "equals".
  
Then - I see the "added number" as the result.

## Scenario: Adding numbers where the result goes out of range

Given - The calculator is ON.

When - I type in "large number"
And I press "plus"
And I type in "large number"
And I press "equals".

Then - I see the added number compacted by using exponent.

## Scenario: 6+* as input

Given - The calculator is ON.

When - I type in "6"
And I press "plus"
And I type in "multiply"
And I press "equals".
  
Then - The output is 6.

## Scenario: Identity operation

Given - The calculator is ON.

When - I type in any number
And I press "plus"
And I type in "0"
And I press "equals".

Then - I see the same number as output.

## Scenario: Converse operation

Given - The calculator is ON.

When - I type second operand
And I press "plus"
And I type in first operand
And I press "equals".

Then - The result is same as addition
of first operand and second operand.
