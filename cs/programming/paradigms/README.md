# Paradigms



**Programming paradigms** are a way to classify [programming languages](https://en.wikipedia.org/wiki/Programming_language) based on their features. Languages can be classified into multiple paradigms.

Some paradigms are concerned mainly with implications for the [execution model](https://en.wikipedia.org/wiki/Execution_model) of the language, such as allowing [side effects](https://en.wikipedia.org/wiki/Side_effect_%28computer_science%29), or whether the sequence of operations is defined by the execution model. Other paradigms are concerned mainly with the way that code is organized, such as grouping a code into units along with the state that is modified by the code. Yet others are concerned mainly with the style of syntax and grammar.



Common programming paradigms include:[\[1\]](https://en.wikipedia.org/wiki/Programming_paradigm#cite_note-1)[\[2\]](https://en.wikipedia.org/wiki/Programming_paradigm#cite_note-2)[\[3\]](https://en.wikipedia.org/wiki/Programming_paradigm#cite_note-symbolic-programming-lisp-3)

* [imperative](https://en.wikipedia.org/wiki/Imperative_programming) in which the programmer instructs the machine how to change its state,
  * [procedural](https://en.wikipedia.org/wiki/Procedural_programming) which groups instructions into procedures,
  * [object-oriented](https://en.wikipedia.org/wiki/Object-oriented_programming) which groups instructions with the part of the state they operate on,
* [declarative](https://en.wikipedia.org/wiki/Declarative_programming) in which the programmer merely declares properties of the desired result, but not how to compute it
  * [functional](https://en.wikipedia.org/wiki/Functional_programming) in which the desired result is declared as the value of a series of function applications,
  * [logic](https://en.wikipedia.org/wiki/Logic_programming) in which the desired result is declared as the answer to a question about a system of facts and rules,
  * [mathematical](https://en.wikipedia.org/wiki/Mathematical_programming) in which the desired result is declared as the solution of an optimization problem
  * [reactive](https://en.wikipedia.org/wiki/Reactive_programming) in which the desired result is declared with data streams and the propagation of change

Declarative programming is when you say _what_ you want, and imperative language is when you say _how_ to get what you want.

A simple example in Python:

```python
# Declarative
small_nums = [x for x in range(20) if x < 5]

# Imperative
small_nums = []
for i in range(20):
    if i < 5:
        small_nums.append(i)
```

The first example is declarative because we do not specify any "implementation details" of building the list.

To tie in a C\# example, generally, using LINQ results in a declarative style, because you aren't saying _how_ to obtain what you want; you are only saying _what_ you want. You could say the same about SQL.

One benefit of declarative programming is that it allows the compiler to make decisions that might result in better code than what you might make by hand. Running with the SQL example, if you had a query like

```text
SELECT score FROM games WHERE id < 100;
```

the SQL "compiler" can "optimize" this query because it knows that `id` is an indexed field -- or maybe it isn't indexed, in which case it will have to iterate over the entire data set anyway. Or maybe the SQL engine knows that this is the perfect time to utilize all 8 cores for a speedy parallel search. _You_, as a programmer, aren't concerned with any of those conditions, and you don't have to write your code to handle any special case in that way.

## References

* [https://en.wikipedia.org/wiki/Programming\_paradigm](https://en.wikipedia.org/wiki/Programming_paradigm)
* [https://www.freecodecamp.org/news/imperative-vs-declarative-programming-difference/](https://www.freecodecamp.org/news/imperative-vs-declarative-programming-difference/)
* [https://www.youtube.com/watch?v=9bW8dp1M1Ac](https://www.youtube.com/watch?v=9bW8dp1M1Ac)

