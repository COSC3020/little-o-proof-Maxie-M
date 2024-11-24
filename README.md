# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

# My Answer, Maxie M. 
- **prove that:** $f(n)\in o(g(n)) \implies f(n) \in O(g(n))$
## Definition of $o(g(n))$
- $f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$
## Definition of O(g(n))$
- $f(n) \in o(g(n)) \iff \exists c' > 0, \exists n_0' , \forall n \geq n_0' : f(n) \leq c' g(n)$
## Proof 
- We will start with $f(n) \in o(g(n))$ by the definition
  - for any $c > 0$, there exists some $n_0$ such that for all $n > n_0, f(n) < cg(n)$
- Once this is completed then, we will compare this this the definition of $O(g(n))$
  - **Big-$O$** requires some positive constant $c'$ and threshold $n'_0$ exist, such that $f(n) \leq c' g(n)$ for all $n \geq n'_0$
  - **Little-$o$** is stricter
    - due to $f(n) < c g(n)$ is required for **any** $c > 0$
- Using the defintion of **o(g(n))$**:
  - can pick any $c' > 0$ (e.g., $c' =1$$
  - find $n_0$ such that $f(n) < c'g(n)$ for all $n \geq n_0$
- **Thus** $f(n) \in O(g(n))
## Conclusion 
- Sticter condition of $o(g(n))$ will guarantee that $f(n)$ also satifies the looser condition of $O(g(n)).
- **Therefore:** $f(n)\in o(g(n)) \implies f(n) \in O(g(n))$
## Plagiarism Statement:
I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
