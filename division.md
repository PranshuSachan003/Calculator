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
  
  Then (I see "negative if any number is negative else positive" as the result)
  
  Scenario: (Division isn't symmetric)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "divide"
And I type in "number"
And I press "equals")
  
  Then (I see the "symmetric property does not hold" as the result)

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
  
  Scenario: (Typing operator more than once )
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "divide"
And I press "divide"
And I type in "number"
And I press "equals")
  
  Then (I see the "divided number" as the result)
  
  Scenario: ( Interleaving of more than one operator)
  
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
  
  Scenario: (Division of more than one number)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "divided"
I type in "number"
And I press "divided"
I type in "number"
And I press "equals")
  
  Then (I see the "divided number according to associativity" as the result)
