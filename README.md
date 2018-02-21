* Negative indexing starts with -1
* `filter(function, sequence)` returns a sequence consisting of those items from the sequence for which function(item) is true
    ~~~
    >>>def f(x): return x % 3 == 0 or x % 5 == 0
    >>> filter(f, range(2, 25))
    [3, 5, 6, 9, 10, 12, 15, 18, 20, 21, 24]
    ~~~
* `map(function, sequence)` calls `function(item)` for each of the sequence’s items and returns a list of the return values
    ~~~
    >>> seq = range(8)
    >>> def add(x, y): return x+y
    ...
    >>> map(add, seq, seq)
    [0, 2, 4, 6, 8, 10, 12, 14]
* `reduce(function, sequence)` returns a single value constructed by calling the binary function function on the first two items of the sequence
    ~~~
    >>> def add(x,y): return x+y
    ...
    >>> reduce(add, range(1, 11))
    55
* When looping through a sequence, the position index and corresponding value can be retrieved at the same time using the `enumerate()` function.
    ~~~
    >>> for i, v in enumerate(['tic', 'tac', 'toe']):
    ...     print i, v
    ...
    0 tic
    1 tac
    2 toe
    ~~~

