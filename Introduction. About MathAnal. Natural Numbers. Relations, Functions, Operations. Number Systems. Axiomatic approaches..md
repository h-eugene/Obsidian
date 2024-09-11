# Material: 
- [Lecture](https://moodle.innopolis.university/pluginfile.php/208410/mod_resource/content/1/MathAnal1fall24.pdf)
- [Lab](https://moodle.innopolis.university/pluginfile.php/210092/mod_resource/content/1/Lab1.pdf)
# Body:
## Basics of naive Set Theory.
### Naive Set Theory postulates existence of:
- the empty set and enumerable sets, an infinite set,
- maps (functions from a set in a set) and power-sets (the sets of all subsets of a set),
- specified subsets by properties,
- unions and Cartesian products of sets.
## The Empty Set, Enumerable Sets, Extensionality:
- There is an empty set $\varnothing$ which has no elements at all: $A \notin \varnothing$ for every set of $A$.
  
- For any infinite collection of sets of $A_{1},\ ...\ A_{n}$ there exists set $\{A_{1},\ ...\ A_{n}\}$ which elements are exactly $A_{1},\ ...\ A_{n}$.
  **Explanation:** In other words, any set is contained in another set.
  
- For all sets of $A$ and $B$, $B\subseteq A$ if $C \in B$ implies $C \in A$ for all $C$; sets are equal when they include each other: $A = B$ if  $A \subseteq B$ if $A \subseteq B$ and $B \subseteq A.$ 
## An (Actual) Infinity:
- There is a set of $\omega$ that:
	- inlcudes the empty set $\varnothing$,
	- with each element $A$ contains a two-element set $\{A, \{A\}\}$: for any $A$, if $A \in \omega$, then $\{A, \{A\}\} \in \omega$.  
## Set Union, Power-set and Specified subset:
- **Definition:** For any set of $A$ there the union ($\cup_{B\in A} B$) is a set which consists of all "elements of elements" in $A$: $C \in (\cup_{B\in A} B)$ if $C \in B$ for some $B \in A$.
  **Explanation:** It's get all unique element from A and if there are nested sets then it discloses them but only first level nested sets.
  **Example:** $A = \{\{1,2\},2,\{3,4\},\{\{2\}\}\}$, then $\cup_{B\in A}B = \{1,2,3,4,\{2\}\}$.     
  
- **Definition:** For any set $A$ the power-set of all his subsets (designation $2^{A}$, $P(A) \ or \ \{B:\ B\subseteq A\}$) is a set.
  **Explanation:** $P(A)$ is set of all subset of set $A$. Count of elements of $P(A)$ is calculated by $2^A$ formula.
  **Example:** Let $A = \{1,2\}$, then $P(A) = \{\varnothing,\{1\},\{2\},\{1,2\}\}$ and quantity of his elements is $2^{2}=4$. 
  
- **Definition:** For any set $A$ and any property $\phi$ (formulated in terms of the naive set theory) collection $\{B:\ B\in A$ and $\phi (B)\}$ is a set (comprising elements of $A$ which enjoy the property $\phi$).
  **Explanation:** $\phi$ - это некоторое условие, по которому отбираются элементы множества $B$ из множества $A$, то есть $B$ это отфильтрованное множество $A$ по условию $\phi$.
  **Example:** $A = \{1,2,3,4,5\},\ \phi(B)$ = "$B$ is a even number." Then:
  $\{B: B\in A$ and $\phi(B)\}$$= \{2,4\}$   
## Optional (to complicated): Axiom of Choice (Cartesian Products):
- For all sets of $A$ and $B$ every total function (correspondence) $F: \ A \rightarrow B$ is a set.
  > [!Help]- Explanation: 
  > $F: \ A\rightarrow B$ means $F(a)\in B$ for each element $a\in A.$ Thus, we get set of elements $\{a,F(a)\ |\ a\in A\}\Leftrightarrow\{a,B\ | \ a\in A\}$. If we will apply this function to each element of $A$ then we get a new set of **ordered pairs**$\{\{a_{1},F(a_{1})\},...,\{a_{n},F(a_{n})\}\ |\ a_{i}\in A\} \Leftrightarrow \{\{a_{1},b_{1}\},...,\{a_{n},b_{n}\}\ |\ a_{i}\in A,\ b_{i}\in B\}.$It's the set of function itself.

- For all sets of $A$ and $B$, any total function $I: \ A \rightarrow B$
  if $I(A)$ doesn't contain the empty set, then there exists the set $\Pi_{C\in A}I(C) \neq \varnothing$ of all functions $F: \ A \rightarrow (\cup_{D\in B}D)$ such that $F(C)\in I(C)$ for every $C \in A.$  
  >[!Help]- Explanation: 
  >1) Let we have set $A$, and each element of this set is also set that not equals to $\varnothing$: $A =\{a,b,c\ \ | \ a=\{..\}\neq\varnothing,\ b=\{..\}\neq\varnothing,\ c=\{..\}\neq\varnothing\}$, then the Axiom of Choice above says that it is possible to choose at least one element from each set of set $A$. 
  2) Function $I: A\rightarrow B$ just explicit show us the set of set A: Let $A=\{a,b\}$ where $a,b,c$ are sets as well and let $a=\{1,2\},\ b=\{3,4\}$, then $I_{C\in A}(C)=\{\{1,2\},\{3,4\}\},\ (I_{C\in A}(C)\Leftrightarrow I(C),\ C\in A)$. And $B=I_{C\in A}(C).$
  >3) $\Pi_{C\in A}I(C) \neq \varnothing$ means *The Cartesian Product* of $I_{C\in A}(C)$ exists and don't equal an empty set, i.e there is at least one combination of elements. For example: Let we have $A = \{a,b\},\ a=\{1,2\},\ b=\{3,4\},$ then $I_{C\in A}(C)=\{\{1,2\},\{3,4\}\},$ and $\Pi_{C\in A}I(C) = \{\{1,3\},\{1,4\},\{2,3\},\{2,4\}\}.$
  > 4) Function $F()$ just maybe functions for selecting some element from each set, I'm not sure because the statement not clear.
  
## Natural Numbers:
- A *natural number* is a measure of the quantity of (indivisible) objects.
- Let $\mathbb{N}$ is the set that satisfies the following two properties:
	- $\mathbb{N}\subseteq \omega, \ \varnothing \in \mathbb{N}$ and with each element $A \in \mathbb{N}$ it contains the set $\{A,\{A\}\};$
	- N is *smallest* collection that satisfies (1) i.e $\mathbb{N} \subseteq M$ for every set $M$ such that $M \subseteq \omega,\ \varnothing \in M$ and with each element $A \in M$ it contains the set $\{A,\{A\}\}$. 
## Constants, predicates and operations on natural numbers:
- Let $0$ be $\varnothing$; if $n$ is defined already then let $(n+1)$ be $\{n,\{n\}\}.$ For example: 1 is $\{\varnothing,\{\varnothing\}\},$ 2 is $\{\{\varnothing,\{\varnothing\}\},\{\{\varnothing,\{\varnothing\}\}\}\},$ etc.
- We can define:
	- predicate $(n=0)$ on $\mathbb{N}$ as $(n = \varnothing);$
	- function (+1): $\mathbb{N}\rightarrow\mathbb{N}$ is $n$ $\mapsto \{n,\{n\}\}$.
## Induction principle and proofs by induction:
- Let $P$ be a monadic predicate (i.e a property of natural numbers):
	- If $0 \in P$ (induction basis),
	- and for $n \in P$ (induction hypothesis) implies $(n+1) \in P$ (induction step) every $n\in \mathbb{N}$
	- then $P = \mathbb{N}$
- The principle follows from the definition of the natural numbers and set theory axiomatic.
## Relations, Functions, Operations:
- Relation (or predicate) on a set $X$ is some subset $Y$ of $X$.
- Examples:
	- natural numbers $p$ and $q$ are co-prime
	- a natural numbers $z$ is a common multiple of two natural numbers $x$ and $y;$
	- a natural number is prime.
## Arity (number of arguments):
- $Y$ is a binary relation on $X_{1}$ and $X_{2}$ if $X$ is Cartesian product of sets $X_1$ and $X_{2}$ (i.e $Y \subseteq X_{1}\times X_{2}$);
- $Y$ is a ternary relation on $X_{1},\ X_{2}$ and $X_{3}$ if $X$ is Cartesian product of sets $X_{1},\ X_{2}$ and $X_{3}$ (i.e $Y \subseteq X_{1}\times X_{2}\times X_{3}$);
- when $X$ isn't a Cartesian product then predicate $Y$ is a monadic pradicate.
## Relations on a set:
- Multi-arity relation on a set is any subset of $X\times ...X=X^{k}\ (k\in \mathbb{N})$. 
  **Explanation:** Just one of all combination with repeations that selects by some property. 
- Binary relation on a set is
	- reflexive if $xRx$ for every x;
	- irreflexive if never $xRx$;
	- symmetric if $xRy$ implies $yRx$ for all $x$ and $y$;
	- transitive if $xRy$ and $yRz$ implies $xRz$ for all $x$,$y$ and $z$
## Equality:
- Reflexive, symmetric and transitive relation is called equivalence.
- Equality is the equivalence that satisfies Leibnitz axiom: $x=y$ iff $\phi(x)\Leftrightarrow \phi(y)$ for every property $\phi.$
## Pre-order, partial and linear order:
- Pre-order (or quasi-order) is a reflexive and transitive relation.
- (Partial) order is an anti-symmetric pre-order, i.e, for any $x$ and $y$, if $xRy$ and $yRx$ then $x=y$.
# Assignments:
- Set up a SciLab
- Explore everything that is unclear: [Математический анализ](V.A.Zorich-Kniga-I-10-izdanie-Corr.pdf)

