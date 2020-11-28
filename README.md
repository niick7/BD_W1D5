# Big Data W1D5

**Instructions**

Q1. Write an in-mapper combiner algorithm modifying Co-occurrence Matrix (pairs approach) algorithm.

**(First you must try. Then look into my solution attached. Trying first is a must.  Use my solution to answer Q3 (b))**

Q2. Write an in-mapper combiner algorithm modifying Co-occurrence Matrix (stripe approach) algorithm.

**(First you must try. Then look into my solution attached. Trying first is a must. Use my solution to answer Q3 (d))**

Q3. Assume that there are two input splits and two reducers. Note that Mapper 1 and Reducer 1 run on the same machine. Mapper 2 and Reducer 2 run on the same machine.

Further, let the partitioner  assign all words less than letter ‘k’ to Reducer 1 and  everything else to Reducer 2.

- Input Split 1 : [ {cat mat rat, cat}, {cat  bat cat pat},{cat bat rat bat}]    (Note : 3 records)

- Input Split 2 : [{cat rat bat rat}, {bat mat pat bat}, {pat cat bat mat}]    (Note: 3 records)

**Let the Window of X be set of all term after X and before the next X.**

Example: Let Data block be [a b c a d e]

Window(a) = {b, c}, Window(b) = {c, a, d, e}, Window(c) = {a, d, e},

Window(a) ={d, e}, Window(d) = {e}, Window(e) = {}.

 
1. Illustrate Pair approach
2. Illustrate In-Mapper Combining Version of the Pair approach. (Use my solution to Q1)
3. Illustrate Stripe approach.
4. Illustrate In-Mapper Combining Version of the Stripe approach. (Use my solution to Q2)
