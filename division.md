# Division

## Scenario: Division by zero when operand one is any number

Given - The calculator is ON

When - I type in "number"
And I press "divide"
And I type in "zero"
And I press "equals"

Then - I see the "Undefined" as result

## Scenario: Divide zero by any number

Given - The calculator is ON

When - I type in "zero"
And I press "divide"
And I type in "number" except "0"
And I press "equals"

Then - I see "zero" as the result

## Scenario: Any one operand is negative

Given - The calculator is ON

When - I type in operand one as positive
And I press "divide"
And I type in operand two as negative
And I press "equals"

Then - I see the "negative number" as the result

## Scenario: Both the operand is negative

Given - The calculator is ON

When - I type in negative number
And I press "divide"
And I type in negative number
And I press "equals"

Then - I see the "positive number" as result

## Scenario: Division isn't symmetric

Given - The calculator is ON

When - I type in "operand two"
And I press "divide"
And I type in "operand one"
And I press "equals"

Then - I see the "number" as result
not same as operand one divide operand two

## Scenario: Division when both operands are 0

Given - The calculator is ON

When - I type in "zero"
And I press "divide"
And I type in "zero"
And I press "equals"

Then - I see the "Undefined" as result

## Scenario: Recurring decimal case

Given - The calculator is ON

When - I type in "number"
And I press "divide"
And I type in "number"
And I press "equals"

Then - I see the "at most five precision" as the result

## Scenario: n number of times "/" pressed

Given - The calculator is ON

When - I type in "number"
And I press "divide"
And I Press "divide"
And I type in "number"
And I press "equals"

Then - I see "divided number" as result.

## Scenario: When operand 2 is not present

Given - The calculator is ON

When - I type in "number"
And I press "divide"
And I press "equals"

Then - I see operand one as result

## Scenario: Division by any/all operands being fractions

Given - The calculator is ON

When - I type in "number"
And I press "divide"
And I type in "fraction number"
And I press "equals"

Then - I see left to right division as result

## Scenario: Division of more than 2 numbers (example: 4/5/6/7)

Given - The calculator is ON

When - I type in "number"
And I press "divide"
And I type in "number"
And I press "divide"
And I type in "number"
And I press "equals"

Then - I see the left to right division as result
