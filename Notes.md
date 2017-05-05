Notes
=====

1. Intro
    1. Overview of talk
        1. What is FP
        2. SOLID applied to FP
        3. My favourite FP language
        4. Some common patterns usable in all languages
2. Quotes
    1. [http://homepages.cs.ncl.ac.uk/brian.randell/NATO/nato1968.PDF
        1. Production of large software has become a scare item for management. By reputation it is often an unprofitable morass, costly and unending.
        2. The good systems that are presently working were written by small groups. More than twenty programmers working on a project is usually disastrous.
        3. There is a widening gap between ambitions and achievements in software engineering ... the gap is arising at a time when the consequences of software failure in all its aspects are becoming increasingly serious
    2. These are from before OO! Maybe it wasn't the saviour we were looking for!
3. What is functional programming?
    1. But how do we do side effects?!
4. Simple vs easy
    1. "Simplicity is the ultimate sophistication" - da Vinci
    2. "Simplicity is a prerequisite for reliability" - Dijkstra
    3. Simple vs complex
        1. Simplex: one fold/braid
        2. Complexus: plaited
    4. Complect: intertwine, to plait together
    5. Don't confuse simple with easy
5. I have no idea what I'm doing
    1. Haven't used FP on a real project
    2. Might just be drinking the Koolaid
    3. But, in the worst case, learning a purely functional programming languages forces you to learn new ways of thinking
    4. I'll try to ground the rant about FP in something familiar - SOLID
6. SOLID:SRP - 'Only do one thing' was taken from imperative programming in the first place. Having small, focused functions is good.
7. SOLID:OCP - Allowing you to change behaviors without modifying code is good. Functional programming uses higher order functions more than inheritance, but the principle holds.
8. SOLID:LSP - Abiding by some interface contract is just as good in functional programming as in object oriented. If a sort function takes a comparator, then you would expect the '0 is equals, less than provides negative results, greater than positive results' behavior.
    1. http://blog.jessitron.com/2013/06/what-fp-taught-me-about-oo-liskov.html
    2. http://gorodinski.com/blog/2013/09/18/oop-patterns-from-a-functional-perspective/
    3. Immutability, parametric polymorphism + laws
9. SOLID:ISP - Most functional languages still have structs. Specifying the smallest set of data required by a function is still good practice. Requiring the least specific interface to the data (why use Lists of ints when Enumerations of T work just as well?) is still good practice.
    1. SRP and ISP lead you to multiple small classes with fine grained interfaces
    2. Such objects represent data with behaviour, but can also be modelled as behaviour with data: Closures. 
10. SOLID:DIP - Specifying parameters to a function (or a higher order function to retrieve them) rather than hard coding the function to go get some value is just as good in functional programming as in object oriented.
11. FP languages
12. Haskell
    1. Here are some reasons why I like Haskell ...
13. Identity function in Haskell
    1. Clean syntax ?
14. Parametricity
    1. Theorems for free - 1989
15. Google & Hayoo
    1. Good tooling
16. Example of program with IO
17. Higher-order functions - map
18. Higher-order functions - filter
19. Higher-order functions - reduce
20. Not a silver bullet
    1. If nothing else, you will learn a different way of thinking


http://www.slideshare.net/firthh/intro-to-functional-programming-levelup-brisbane

make illegal states unrepresentable - http://rea.tech/the-abject-failure-of-weak-typing/

1. Lazy evaluation
    1. http://blog.tmorris.net/posts/what-is-haskells-primary-feature/index.html


https://www.google.com.au/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=haskell%20pure%20tests

http://stackoverflow.com/questions/7370073/testing-functions-in-haskell-that-do-io


SOLID
1. http://programmers.stackexchange.com/questions/165356/equivalent-of-solid-principles-for-functional-programming
2. http://blog.ploeh.dk/2014/03/10/solid-the-next-step-is-functional/


Why FP matters
* https://www.mendeley.com/viewer/?fileId=2bdf50e5-8d1b-8fff-726f-6d9652407785&documentId=ab4fa60b-4d07-3761-a762-6f18378ee162
* As software becomes more and more complex, it is more and more important to structure it well. Well-structured software is easy to write and to debug, and provides a collection of modules that can be reused to reduce future programming costs. In this paper we show that two fea-tures of functional languages in particular, higher-order functions and lazy evaluation, can contribute significantly to modularity. As examples, we manipulate lists and trees, program several numerical algorithms, and implement the alpha-beta heuristic (an algorithm from Artificial Intelligence used in game-playing programs). We conclude that since modularity is the key to successful programming, functional programming offers important advantages for software development.

Out of the Tar Pit
* Complexity is the single major difficulty in the successful develop-ment of large-scale software systems. Following Brooks we distinguish accidentalfromessential difficulty, but disagree with his premise that most complexity remaining in contemporary systems is essential. We identify common causes of complexity and discuss general approaches which can be taken to eliminate them where they are accidental in nature.  To make things more concrete we then give an outline for a potential complexity-minimizing approach based on functional pro-grammingandCodd's relational model of data