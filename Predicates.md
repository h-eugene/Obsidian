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