# Basic Elements:

> [!abstract] Set
> An unordered  collection of things (not counting multiplicities), its elements.
> **Descriptions:**
> *List* $X = \{x_{1},x_{2},...,x_{n}\}$
> *Rule* $X= \{x|$ some condition on $x$ holds$\}$

> [!abstract] Membership
> $a\in X$ – "$a$ is an element of $X$"
> $\neg(a\in X)\rightleftharpoons a \notin X$
> 
> *$\rightleftharpoons$ means "by definition" 

>[!abstract] Proposition
>A sentence (that declares a fact) that is either *true* or *false*, but not both.

>[!abstract] Predicate $P\{x_1,...,x_{n}\}$
>A sentence with parameters $x_{1} \in D_{1},...,x_{n}\in D_{n}$ (its truth depends on $x_1,...,x_n$)
>
>The set $D_{1}\times ... \times D_{n}$ is called the ***domain*** of $P$

>[!abstract] Quantifiers (some denotions)
>The universal quantifiers|The existential quantifier
>--|--
>"for Any", "for All"|"Exists" 
>$\forall x\ P(x)$|$\exists x \ P(x)$

>[!abstract] Bound and Free occurrence
>- Every occurrence of a variable $x$ in a formula of the form $\exists x \ P(x)$ or of the form $\forall x \ P(x)$ is called a ***bound*** occurrence.
>- Occurrences which are not *bound* are called ***free***.  
>  
>  **Example:**
>  $$P(z)=\exists x ((z\neq x)\rightarrow \forall y((y=z)\vee (y=x)))$$ 
>  Bound: $x,y$
>  Free: $z$

>[!info] Fact
>If a formula does not contain free variables then it becomes a *proposition*. (Its truth still depends on the domain.)

> [!abstract] Interpretation
> An (positive) ***interpretation*** for a formula of predicate logic is possible meanings for domain, predicates and variables such that a truth value of the formula becomes *TRUE*.
> 
> **Example:**
> Let the domain consist of all natural numbers.
> $P(x)=$ "$x$ is even"
> Therefore, $\exists x \ P(x) =$ "There is an even number"  
> 
> Let the domain consist of all natural numbers dividing by 4.
> $P(x) =$ "$x$ is even"
> Therefore, $\forall x\ P(x) =$ "Any natural number dividing by 4 is divided by 2"
> 

>[!abstract] Counterexample
>A counterexample for a formula of predicate logic is possible meanings for domain, predicates and variables such that a truth value of the formula becomes *FALSE*.
>
>**Example:**
>Let the domain consist of all people.
>$P(x) =$ "$x$ can fly"
>Therefore, $\forall x \ P(x) =$ "Anyone can fly"

# De Morgan's Laws:

>[!abstract] Definition
>$\neg \forall x \ P(x)\equiv \exists x \neg P(x)$
>$\neg \exists x \ P(x) \equiv \forall x \neq P(x)$

>[!check]  Interpretation
>Let the domain consist of all natural numbers and $P(x) =$ "$x$ is even".
>$$\forall x\ P(x) = \text{"any natural number is even"}$$ 
>$$\neg \forall x \ P(x) = \text{"not any natural number is even}$$
>$$\exists x \neg P(x) = \text{"there exists a natural number which is not even"}$$