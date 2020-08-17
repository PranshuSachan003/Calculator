Subtraction

Scenario: ( Subtraction of two positive numbers)

Given (The calculator turns on)

When (I type in "positive number" And I press "minus" And I type in "positive number" And I press "equals")

Then (I see the "subtracted number" as the result)

Scenario: ( Subtraction of two negative numbers)

Given (The calculator turns on)

When (I type in "negative number" And I press "minus" And I type in "negative number" And I press "equals")

Then (I see the "subtracted number" as the result)

Scenario: ( Subtraction of two fraction numbers)

Given (The calculator turns on)

When (I type in "fraction number" And I press "minus" And I type in "fraction number" And I press "equals")

Then (I see the "subtracted number" as the result)

Scenario: (Subtraction of positive and negative number)

Given (The calculator turns on)

When (I type in "positive number" And I press "minus" And I type in "negative number" And I press "equals")

Then (I see the "subtracted number" as the result)

Scenario: (Subtraction of decimals)

Given (The calculator turns on)

When (I type in "decimal number" And I press "minus" And I type in "decimal number" And I press "equals")

Then (I see the "subtracted number" as the result)

Scenario: (Typing operator more than once)

Given (The calculator turns on)

When (I type in "number" And I press "minus" And I press "minus" And I type in "number" And I press "equals")

Then (I see the "subtracted number" as the result)

Scenario: (Subtraction of more than 2 numbers)

Given (The calculator turns on)

When (I type in "number" And I press "minus" And I type in "number" And I press "minus" And I type in "number" And I press "equals")

Then (I see the "subtracted number" as the result)

Scenario: ( Subtraction of numbers where the result goes out of range)

Given (The calculator turns on)

When (I type in "number" And I press "minus" And I type in "number" And I press "equals")

Then (I see the "out of range" as the result)

Scenario: (number-*number is provides as input)

Given (The calculator turns on)

When (I type in "number" And I press "minus" And I press "multiply" And I press "equals")

Then (I see the "multiplied number" as the result)

Scenario: (Subtraction of number with zero)

Given (The calculator turns on)

When (I type in "number" And I press "minus" And I press "zero" And I press "equals")

Then (I see the "same number" as the result)
