# Addition

Scenario: (describe a scenario here)
  
  Given (state the initial condition)
  
  When (state the event)
  
  Then (state the effect)
  
Scenario: Addition of two positive numbers
  
  Given - The calculator is turned on.

  When -  I type in "positive number"
          And I press "plus"
          And I type in "positive number"
          And I press "equals"
  
  Then - I see the "added number" as the result.


  
Scenario: Addition of two negative numbers
  
  Given - The calculator is turned on.

  When - I type in "negative number"
          And I press "plus"
          And I type in "negative number"
          And I press "equals".
  
  Then - I see the "added number" as the result which is also a negative number.
  
Scenario: Addition of fractions
  
  Given - The calculator is turned on.

  When - I type in "numerator followed by division sign followed by denominator"
          And I press "plus"
          And I type in "numerator followed by division sign followed by denominator"
          And I press "equals".
  
  Then - I see the "added number" as the result.
  
Scenario: Addition of positive and negative number
  
  Given - The calculator is turned on.

  When - I type in "positive number"
          And I press "plus"
          And I type in "negative number"
          And I press "equals".
  
  Then - I see the "added number" as the result.
  
Scenario: Addition of decimals
  
  Given - The calculator is turned on.

  When - I type in "decimal number"
          And I press "plus"
          And I type in "decimal number"
          And I press "equals".
  
  Then - I see the "added number" as the result.
  
Scenario: Typing operator more than once
  
  Given - The calculator is turned on.

  When - I type in "positive or negative number"
          And I press "plus"
          And I type in "plus"
          And I press "equals".
  
  Then - The result is the same number given as input.
  
Scenario: Addition of more than 2 numbers
  
  Given - The calculator is turned on.

  When - I type in "postive number or negative number"
          And I press "plus"
          And I type in "positive number" or "negative number in braces"
          And I press "plus"
          And I type in "positive number" or "negative number in braces"
          And I press "equals".
  
  Then - I see the "added number" as the result.
  
Scenario: Adding numbers where the result goes out of range
  
  Given - The calculator is turned on.

  When - 
  
  Then -  
  
Scenario: 6+* is provided as input?
  
  Given - The calculator is turned on.

  When - I type in "6"
          And I press "plus"
          And I type in "multiply"
          And I press "equals".
  
  Then - The output is 6.
  
