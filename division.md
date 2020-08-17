# Division

Scenario: (Division by 0 when operand 1 is any number)
  
  Given (The calculator turns on)

  When (I type in "number"
And I press "divide"
And I type in "zero"
And I press "equals")
  
  Then (I see the "undefined" as the result)

Scenario: ( Divide 0 by any number)
  
  Given (The calculator turns on)
  
  When (I type in "zero"
And I press "divide"
And I type in "number"
And I press "equals")
  
  Then (I see the "zero" as the result)

Scenario: ( Sign rules for operands)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "divide"
And I type in "number"
And I press "equals")
  
  Then (I see the "divided number with negative sign if any number is negative 
  else with positive sign" as the result)
  
  Scenario: (Division isn't symmetric)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "divide"
And I type in "number"
And I press "equals")
  
  Then (I see the "by reversing these two number 
  divided number is not same" as the result)

Scenario: (Division when both operands are 0)
  
  Given (The calculator turns on)
  
  When (I type in "zero"
And I press "divide"
And I type in "zero"
And I press "equals")
  
  Then (I see the "undefined" as the result)
  
  Scenario: (Recurring decimal case)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "divide"
And I type in "number"
And I press "equals")
  
  Then (I see the "in divided number after decimal digit is repeating" as the result)
  
  Scenario: (Multiple times "/" is pressed)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "divide"
And I press "divide"
And I type in "number"
And I press "equals")
  
  Then (I see the "divided number" as the result)
  
  Scenario: ( Interleaving of multiple operators)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "plus"
And I press "divide"
And I press "another operator"
And I press "another operator"
And I type in "number"
And I press "equals")
  
  Then (I see the "number according to last operator" as the result)
  
   Scenario: ( When operand 2 is not present)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "divided"
And I press "equals")
  
  Then (I see the "number" as the result)
  
  Scenario: (Division by any/all operands being fractions)
  
  Given (The calculator turns on)
  
  When (I type in "fraction number"
And I press "divided"
I type in "fraction number"
And I press "equals")
  
  Then (I see the "divided number" as the result)
  
  Scenario: (Division of multiple numbers (eg: 4/5/6/7))
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "divided"
I type in "number"
And I press "divided"
I type in "number"
And I press "equals")
  
  Then (I see the "divided number according to associativity" as the result)
