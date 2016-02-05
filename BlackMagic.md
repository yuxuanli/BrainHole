## BalckMagic

1. What is the difference between `String one = "one";` and `String one=new String("one");`?
Ans: There is one thing in Java called "String literal pool", in order to cut down the number of String object create in JVM.
By using `String one="one";`, if there is already a "one" String in the pool, it will return the reference to variable a, otherwise it will create a new string object and put it into the pool.
While if you are using `String one=new String("one");`, it will always create a new String object outside the pool, no matter if a duplicated string over there in the pool.

2. Why not use double or int in currency calculation?
Ans: http://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency

3. What is the difference between the operators `>>>` and `>>` in Java?
Ans: The unsigned right shift operator ">>>" shifts a zero into the leftmost position, while the leftmost position after ">>" depends on sign extension.

4. What if the difference between `Abstraction` and `Encapsulation` and `Information Hidding`?
Ans: http://stackoverflow.com/questions/24626/abstraction-vs-information-hiding-vs-encapsulation/8694874#8694874
Abstraction is kind of technology that decide what is the commmon thing among these items, and observe them in a high level.
Encapsulation is kind of technology hide what should be hide and rule the method of iteracting with internal attribute.
Information hidding is just a method of encapsulation, but no all of it.
