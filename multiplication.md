# Multiplication

## Scenario: Result overflow

Given - The calculator is ON.

When - I type a large number
And I press "multiply"
And I type another large number
And I press "equals"

Then - I see a large number with
exponent in the end.

## Scenario: Signs of the numbers

Given - The calculator is ON.

When - I type any number
And I press "multiply"
And I type another number
And I press "equals"

Then - I see the result as multiplied number with
relative sign.

## Scenario: Zero value multiplication

Given - The calculator is ON.

When - I type "0"
And I press "multiply"
And I type any number
And I press "equals"

Then - I see the result "0".

## Scenario: Multiplication by 1

Given - The calculator is ON.

When - I type "1"
And I press "multiply"
And I type any number
And I press "equals"

Then - I see original number as result.

## Scenario: Decimal value multiplication

Given - The calculator is ON.

When - I type any decimal number
And I press "multiply"
And I type another decimal number
And I press "equals"

Then - I see the result as "multiplied number" up to
five decimal places except if "0".

## Scenario: Irrational value multiplication

Given - The calculator is ON.

When - I type any irrational number
And I press "multiply"
And I type another irrational number
And I press "equals"

Then - I see the result as "multiplied number" up to
five decimal places except if "0".

## Scenario: Simple multiplication

Given - The calculator is ON.

When - I type any number
And I press "multiply"
And I type another number
And I press "equals"

Then - I see the result as "multiplied number".

## Scenario: Rational multiplication

Given - The calculator is ON.

When -  I type any rational number
And I press "multiply"
And I type another rational number
And I press "equals"

Then - I see the result as "multiplied number" up to
five decimal places except if "0".

## Scenario: Decimal & integer multiplication

Given - The calculator is ON.

When - I type any decimal number
And I press "multiply"
And I type another rational number
And I press "equals"

Then - I see the result as "multiplied number" up to
five decimal places except if "0".

## Scenario: More than two numbers multiplication

Given - The calculator is ON.

When - I type numbers with "multiply" as operator.

Then - I see the result as "multiplied number".

## Scenario: Complex number multiplication

Given - The calculator is ON.

When - I press "Ci" for Complex number computation
And I type in "complex number"
And I press "multiply"
And I type in "complex number or real number"
And I press "equal"

Then - I see "multiplied number" as the result.

## Scenario: Range of operand exceeds allowed limit

Given - The calculator is ON.

When - I type an operand which exceeds limit

Then - Stop taking more digits.

## Scenario: Pressing "multiply button" many times

Given - The calculator is ON.

When - I type any number
And I press "multiply" many times

Then - I see multiply sign comes once.

## Scenario: Interleaving operators (Press *, then press /, then press +)

Given - The calculator is ON.

When - I type any number
And I press "multiply"
And I type any number
And I press "divide"
And I type any number
And I press "plus"
And I type any number
And I press "equals"

Then - I see the result after computing from left
to right.
