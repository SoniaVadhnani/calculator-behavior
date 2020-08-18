# Subtraction

## Scenario: Subtraction of two positive numbers

Given - The calculator is ON

When - I type in "positive number"
And I press "minus"
And I type in "positive number"
And I press "equals"

Then - I see the "subtracted number" as the result

## Scenario: Subtraction of two negative numbers

Given - The calculator is ON

When - I type in "negative number"
And I press "minus"
And I type in "negative number"
And I press "equals"

Then - I see the "subtracted number" as the result

## Scenario: Subtraction of fractions

Given - The calculator is ON

When - I type in "fraction number"
And I press "minus"
And I type in "fraction number"
And I press "equals"

Then - I see the "subtracted number" as the result

## Scenario: Subtraction of positive and negative number

Given - The calculator is ON

When - I type in "positive number"
And I press "minus"
And I type in "negative number"
And I press "equals"

Then - I see the "subtracted number" as the result

## Scenario: Subtraction of decimals

Given - The calculator is ON

When - I type in "decimal number"
And I press "minus"
And I type in "decimal number"
And I press "equals"

Then - I see the "subtracted decimal number" as result

## Scenario: Typing operator more than once

Given - The calculator is ON

When - I type in "number"
And I press "minus"
And I press "minus"
And I type in "number"
And I press "equals"

Then - I see the "subtracted number" as result as it
take second operator as sign of next operand

## Scenario: Subtraction of more than two numbers

Given - The calculator is ON able to enter number

When - I type in "number"
And I press "minus"
And I type in "number"
And I press "minus"
And I type in "number"
And I press "equals"

Then - I see the "subtracted number" as result
from left to right

## Scenario: Subtracting numbers where the result goes out of range

Given - The calculator is ON

When - I type in "large number"
And I press "minus"
And I type in "large number"
And I press "equals"

Then - I see the result in compact
form with exponent

## Scenario: 6-* as input

Given - The calculator is ON

When - I type in "number"
And I press "minus"
And I press "multiply"
And I press "plus"
And I press "equals"

Then - I see "6" as result

## Scenario: Identity operation

Given - The calculator is ON able to enter number

When - I type in any number
And I press "minus"
And I type in "0"
And I press "equals"

Then - I see the same number as output

## Scenario: Converse operation

Given - The calculator is ON

When - I type in "operand two"
And I press "minus"
And I type in "operand one"
And I press "equals"

Then - I see the "subtracted number" as result
