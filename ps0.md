# CS 121 Homework Zero: Fall 2019

The aim of problem set is to help you in brushing up on the mathematical background needed to be successful in CS 121. This problem set will be due in the first week of class, but I encourage you to start working on it over the summer. 


__Some policies:__ (See the [course syllabus](http://cs121.boazbarak.org/syllabus/) for the full policies.)

* You can collaborate with other students that are currently enrolled in this course  (or, in the case of homework zero, planning to enroll in this course) in brainstorming and thinking through approaches to solutions but you should write the solutions on your own and cannot share them with other students. 

* Always make sure that you "own" your solutions to this other problem sets. That is, you should always first grapple with the problems on your own, and even if you participate in brainstorming sessions, make sure that you completely understand the ideas and details underlying the solution. This is in your interest as it ensures you have a solid understanding of the course material, and will help in the midterms and final. There will be many "bonus points" in the problem sets and ways to make up for lost points. Therefore getting 80% of the problem set questions right on your own will be much better to both your understanding and grade than getting 100% of the questions through gathering hints from others without true understanding.

* Sharing questions or solutions with anyone outside this course, including posting on outside websites, is a violation of the honor code policy. Collaborating with anyone except students currently taking this course or using material from past years from this or other courses is a violation of the honor code policy.

* The submitted PDF should be typed and in the same format and pagination as ours. Please include the text of the problems and write __Solution X:__ before your solution. (This is easy to do if you use our markdown template.) Please mark in gradescope the pages where the solution to each question appears. Points will be deducted if you submit in a different format.


**By writing my name here I affirm that I am aware of all policies and abided by them while working on this problem set:** 

__Your name:__ (Write name and HUID here)

__Collaborators:__ (List here names of anyone you discussed problems or ideas for solutions with)

\newpage




## Questions


Please solve the following problems. Some of these might be harder than the others, so don't despair if they require more time to think or you can't do them all. Just do your best. Also, you should only attempt the bonus questions if you have the time to do so.
If you don't have a proof for a certain statement, be upfront about it.
You can always explain clearly what you are able to prove and the point at which you were stuck.
Also, for a non bonus question, you can always simply write __"I don't know"__ and you will get 15 percent of the credit for this problem.

The Piazza board for this course will be active even before the course starts. If you are stuck on this problem set, you can use Piazza to send a private message to all instructors under the `e-office-hours` folder.

This problem set has a total of __50 points__ and __11 bonus points__. A grade of 50 or more on this problem set is considered a perfect grade. If you get stuck in any questions, you might find the resources in the [CS 121 background page](https://cs121.boazbarak.org/background/) helpful.

__Problem 0 (5 points):__ Read fully the __Mathematical Background Chapter__ ( [pdf format](https://introtcs.org/public/lec_00_1_math_background.pdf)
[html format](https://introtcs.org/public/lec_00_1_math_background.html)  ) from the textbook on the website [https://introtcs.org](https://introtcs.org). This is probably the most important exercise in this problem set!!


__Solution 0:__ (Write "I certify that I fully read the mathematical background chapter".)

I certify that I fully read the mathematical background chapter


### Logical operations, sets, and functions

These questions assume familiarity with strings, functions, relations, sets, and logical operators.
We use an indexing from zero convention, and so given a length $n$ binary string $x\in \{0,1\}^n$, we denote coordinates of $x$ by $x_0,\ldots,x_{n-1}$.
We use $[n]$ to denote the set $\{0,1,\ldots,n-1\}$.


__Question 1 (3 points):__ Write a logical expression $\varphi(x)$ involving the variables $x_0,x_1,x_2$ and the operators $\wedge$ (AND), $\vee$ (OR), and $\neg$ (NOT), such that $\varphi(x)$ is true if and only if the majority of the inputs are _False_.

__Solution 1:__

$\varphi(x) = (\neg (x_0 \vee x_1)) \vee (\neg (x_0 \vee x_2)) \vee (\neg (x_1 \vee x_2))

__Question 2:__ Use the logical quantifiers $\forall$ (for all), $\exists$ (exists), as well as $\wedge,\vee,\neg$ and the arithmetic operations $+,\times,=,>,<$ to write the following:

__Question 2.1 (3 points):__ An expression $\psi(n,k)$ such that for every natural numbers $n,k$, $\psi(n,k)$ is true if and only if $k$  divides $n$.

__Solution 2.1:__

__Question 2.2 (3 points bonus):__ An expression $\varphi(n)$ such that for every natural number $n$, $\varphi(n)$ is true if and only if $n$ is a power of three.

__Solution 2.2:__


__Question 3:__ In this question, you need to describe in words sets that are defined using a formula with quantifiers. For example, the set $S = \{ x\in \mathbb{N} \;:\; \exists_{y\in\mathbb{N}} x=2y \}$ is the set of even numbers.

__Question 3.1 (3 points):__ Describe in words the following set $S$:

$$
S = \{ x\in \{0,1\}^{100} : \forall_{i\in \{0,\ldots, 98\}} x_i = x_{i+1} \}
$$

(Recall that, as written in the mathematical background chapter, we use zero-based indexing in this course, and so a string $x\in \{0,1\}^{100}$ is indexed as $x_0x_1\cdots x_{99}$.)

__Solution 3.1:__

__Question 3.2 (3 points):__ Describe in words the following set $T$:

$$
T = \{ x\in \{0,1\}^* : |x|>1 \text{ and } \forall_{i \in \{2,\ldots,|x|-1 \} } \forall_{j \in \{2,\ldots,|x|-1\}} i\cdot j \neq |x| \}
$$


__Solution 3.2:__



__Question 4:__ This question deals with sets, their cardinalities, and one to one and onto functions. You can cite  results connecting these notions from the course's textbook, MIT's "Mathematics for  Computer Science" or any other discrete mathematics textbook.

__Question 4.1 (4 points):__ Define $S = \{0,1\}^6$ and $T$ as the set $\{ n \in [100] \;|\; \text{$n$ is prime } \}$.
_Prove or disprove:_ There is a one to one function from $S$ to $T$.

__Solution 4.1:__


__Question 4.2 (4 points):__
Let $n=100$, $S = [n] \times [n] \times [n]$ and $T=\{0,1\}^n$.
_Prove or disprove:_ There is an onto function from $T$ to $S$.

__Solution 4.2:__


__Question 4.3 (4 points):__ Let $n=100$, let $S = \{0,1\}^{n^3}$ and $T$ be the set of all functions mapping $\{0,1\}^n$ to $\{0,1\}$.
_Prove or disprove:_ There is a one to one function from $S$ to $T$.

__Solution 4.3:__


__Question 5.1 (5 points):__  Prove that for every finite sets $A,B,C$, $|A \cup B \cup C| \leq |A|+|B|+|C|$.

__Solution 5.1:__

__Question 5.2 (5 points bonus):__ Prove that for every finite sets $A,B,C$, $|A \cup B \cup C| \geq |A|+|B|+|C| - |A \cap B| - |B \cap C| - |A \cap C|$.

__Solution 5.2:__



### Graphs

Thee following two questions assume familiarity with basic graph theory. If you need to look up or review any terms, the [CS 121 background page](https://cs121.boazbarak.org/background/)  contains several freely available online resources on graph theory. This material also appears in Chapters 13,14,16 and 17 of the CS 20 textbook "Essential Discrete Mathematics for Computer Science" by Harry Lewis and Rachel Zax.

__Question 6.1 (5 points):__ Prove that if $G$ is a directed acyclic graph (DAG) on $n$ vertices, if $u$ and $v$ are two vertices of $G$ such that there is a directed path of length $n-1$ from $u$ to $v$ then $u$ has no in-neighbors.^[_Hint:_ You can use the topological sorting theorem shown in the mathematical background chapter.]


__Solution 6.1:__


__Question 6.2 (5 points):__ Prove that for every undirected graph $G$ of $1000$ vertices, if every vertex has degree at most $4$, then there exists a subset $S$ of at least $200$ vertices such that no two vertices in $S$ are neighbors of one another.

__Solution 6.2:__


### Big-O Notation 


__Question 7:__  For each pair of functions $f,g$ below, state whether  or not $f=O(g)$ and  whether or not $g=O(f)$.


__Question 7.1 (3 points):__  $f(n)=n(\log n)^3$ and $g(n)=n^2$.

__Solution 7.1:__


__Question 7.2 (3 points):__ $f(n)= n^{\log n}$ and $g(n) = n^2$.

__Solution 7.2:__


__Question 7.3 (3 points bonus):__ $f(n) = \binom{n}{\lceil 0.2 n \rceil}$ (where $\binom{n}{k}$ is the number of $k$-sized subsets of a set of size $n$) and $g(n) = 2^{0.1 n}$.^[_Hint:_ one way to do this is to use [Stirling's approximation](https://goo.gl/cqEmS2).]

__Solution 7.3:__
