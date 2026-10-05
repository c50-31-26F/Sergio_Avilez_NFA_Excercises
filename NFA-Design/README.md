*NFA Design Exercises — Problems 6–10

6- Strings that start with `10`
7- Strings that end with `10`
8- Strings that start with `01` and end with `10`
9- Strings that contain substring `10`
10- Strings that do not contain substring `10`

1. Which problems gave me the most trouble?

Problems 7–9 required more thought than Problem 6 because the NFA has to use nondeterminism to search for a pattern. Problem 8 was interesting because it combines a required beginning "01" with a required ending "10".

I asked AI for help understanding how to design the states and how nondeterministic paths work. I also used JFLAP to verify the designs instead of assuming that my diagram was correct.

2. Gold-st-ring and unexpected next states

The biggest surprise I encountered was remembering that an NFA can have more than one possible current state after reading the same input. For example, in the NFA for a string ending in "10", the machine can stay in its searching state while also taking a transition that guesses the beginning of the final "10".

This means I need to think in terms of a "set of possible states", not one state. When checking a difficult string, I should list all possible states after every input symbol.

3. Other insights

The problems helped me see the difference between several common NFA patterns:
It starts with a pattern to force the first transitions and it also ends with a pattern, but it can also end with no accepting patterns which I thought was interesting. 

I find JFLAP's Multiple Run feature is useful because it can quickly check many examples at once. I do need to practice with it a little more since the problems I did were very simple due to time constraints.
