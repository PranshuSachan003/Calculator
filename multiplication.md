# Multiplication

Scenario: (Simple multiplication)
 
  Given (The calculator turns on)

  When (I type in "number"
And I press "multiply"
And I type in "number"
And I press "equals")
  
  Then (I see the "multiplied number" as the result)

Scenario: ( Rational multiplication)
  
  Given (The calculator turns on)
  
  When (I type in "rational number"
And I press "multiply"
And I type in "rational number"
And I press "equals")
  
  Then (I see the "multiplied number" as the result)

Scenario: ( Result overflow)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "multiply"
And I type in "number"
And I press "equals")
  
  Then (I see the "out of range" as the result)
  
  Scenario: (Signs of the numbers)
  
  Given (The calculator turns on)
  
  When (I type in "positive number"
And I press "multiply"
And I type in "negative number"
And I press "equals")
  
  Then (I see the "minus sign with multiplied number" as the result)

Scenario: (Zero value multiplication)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "multiply"
And I type in "zero"
And I press "equals")
  
  Then (I see the "zero" as the result)
  
  Scenario: (Multiplication by 1)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "multiply"
And I type in "one"
And I press "equals")
  
  Then (I see the "number" as the result)
  
  Scenario: (More than two numbers multiplication)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "multiply"
And I type in "number"
And I press "multiply"
And I type in "number"
And I press "equals")
  
  Then (I see the "multiplied number" as the result)
  
  Scenario: ( Decimal value multiplication)
  
  Given (The calculator turns on)
  
  When (I type in "decimal number"
And I press "multiply"
And I type in "decimal number"
And I press "equals")
  
  Then (I see the "multiplied number" as the result)
  
   Scenario: ( Irrational value multiplication)
  
  Given (The calculator turns on)
  
  When (I type in "irrational number"
And I press "multiply"
And I type in "irrational number"
And I press "equals")
  
  Then (I see the "multiplied number" as the result)
  
  Scenario: (Decimal & integer multiplication)
  
  Given (The calculator turns on)
  
  When (I type in "decimal number"
And I press "multiply"
And I type in "integer number"
And I press "equals")
  
  Then (I see the "multiplied number with decimal" as the result)
  
  Scenario: (Complex number multiplication)
  
  Given (The calculator turns on)
  
  When (I type in "Complex number"
And I press "multiply"
And I type in "Complex number"
And I press "equals")
  
  Then (I see the "Complex multiplied number" as the result)
  
  Scenario: (Range of operand exceeds allowed limit)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "multiply"
And I type in "number"
And I press "equals")
  
  Then (I see the "out of range" as the result)
  
  Scenario: (Pressing "multiply button" more than one time)
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "multiply"
And I press "multiply"
And I type in "number"
And I press "equals")
  
  Then (I see the "multiplied number" as the result)
  
  Scenario: (Interleaving operators (Press *, then press /, then press +))
  
  Given (The calculator turns on)
  
  When (I type in "number"
And I press "multiply"
And I press "divide"
And I type in "Plus"
And I type in "number"
And I press "equals")
  
  Then (I see the "added number" as the result)
  
  Scenario: (Decimal value capping)
  
  Given (The calculator turns on)
  
  When (I type in "decimal number"
And I press "multiply"
And I type in "decimal number"
And I press "equals")
  
  Then (I see the "multiplied number with fixed digits after decimal" as the result)
