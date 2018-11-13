# Methods of Optimization
**Study Project 2018**
 **Authors**: Krivoshapko Mariya, Kudryavtseva Polina, Anisimova Victoria

----------------------------------------------------------------------
## Task
Let us recall the statement of problem. 

Let $X \in \{0,1\}$ be a random variable, that satisfies $$prob(X=1) = p = \frac {exp(a^{T}x+b)}{1+exp(a^{T}x+b)} $$  where $x \in \mathbb{R}^n$ is a vector of variables that affect the probability, and $a$ and $b$ are known parameters. We can think of $X = 1$ as the event that a consumer buys a product, and $x$ as a vector of variables that affect the probability, e.g., advertising effort, retail price, discounted price, packaging expense, and other factors. 
The variable $x$, which we are to optimize over, is subject to a set of linear constraints, $Fx \preceq g$.

Our goal is to maximize 

* buying probability
* expected profit

-------------------------------------------------------------
## Problem Restatement

As we have already seen, both of these problems can be reformulated as problems of convex optimiztion. 

Indeed, the first problem here is equivalent to maximization of $a^T x$ subject to $Fx \preceq g$
The second problem is  maximization of expected profit's natural logarithm, i.e.: $$a^T x + b − \ln (1 + exp(a^T x + b) ) + \ln(c^T x + d)$$ subject to $Fx \preceq g$

---------------------------------------
## Methods Implemented
Following methods are going to be implemented in our project

### First-order Methods
* Projected gradient descent
* Probably conditional gradient descent (after deadline)
* Probably stochastic gradient descent (after deadline)

### Second-Order Methods

### Quasi-Newton Methods

### Inner Point Method
