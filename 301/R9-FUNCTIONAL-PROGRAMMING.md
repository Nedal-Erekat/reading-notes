# Functional programming
#### Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data
1.  pure functions
 * It returns the same result if given the same arguments
 * It does not cause any observable side effects
 > - If our function reads external files, it’s not a pure function — the file’s contents can change.
 - Any function that relies on a random number generator cannot be pure.

2. Immutability
#### Unchanging over time or unable to be changed. When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

#### With *recursion*, we keep our variables immutable. The list and the accumulator variables are not changed. It keeps the same value.

3. Referential transparency
#### We can replace the entire expression with a numerical constant and memoize it.

4. Functions as first-class entities
- Functions as first-class entities can:
 - refer to it from constants and variables
 - pass it as a parameter to other functions
 - return it as result from other functions

5. Higher-order functions

#### When we talk about higher-order functions, we mean a function that either:
 - takes one or more functions as arguments, or
 - returns a function as its result
