# Addition

Scenario: (Addition of two positive numbers)
  
  Given (The calculator turns on)

  When (I type in "positive number"
And I press "plus"
And I type in "positive number"
And I press "equals")
  
  Then (I see the "added number" as the result)

Scenario: ( Addition of two negative numbers)
  
  Given (The calculator turns on)
  
  When (I type in "negative number"
And I press "plus"
And I type in "negative number"
And I press "equals")
  
  Then (I see the "added number" as the result)
