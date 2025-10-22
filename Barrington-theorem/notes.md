# Links, resources

[Barrington's paper](https://people.cs.umass.edu/~barring/publications/bwbp.pdf)
[NC complexity class](https://en.wikipedia.org/wiki/NC_(complexity))
[Boneh's note on Barrington's theorem](https://crypto.stanford.edu/~dabo/pubs/papers/barrington.html)


# Preliminaries

* $\textsf{NC}^i$: set of decision problems decidable in polylogarithmic time $\mathcal{O}((\log n)^i)$ on a parallel computer with a polynomial number of processors. A problem with input size `n` is in NC if $\exists\,c,k\colon$it can be solved in time $\mathcal{O}((\log n)^c)$ using $\mathcal{O}(n^k)$ parallel processors.
* Example of problem in $\textsf{NC}^1$: parity check of a bit string, i.e, decide whether the number of `1` bits is even or odd. This can be obtained by performing the exclusive or ($\oplus$) of all bits. Since $\oplus$ is symmetric and associative, we can solve in parallel in $\log n$ steps (circuit depth) with $n-1$ total XORings (circuit size).
* A language $L$ is defined as a set of strings chosen from all possible finite sequences of symbols over a given alphabet $\Sigma$ (e.g., $\Sigma =\{0,1\}$\). A language can be used to represent a decision problem. For example, the parity check problem can be defined as the language $L_{parity}$ over the alphabet $\{0,1\}$ containing all strings with an odd number of 1s:

$$
L_{parity}=\{w\in \{0,1\}^{*}\mid \oplus_{i} w_i  = 1\}
$$

* A **branching program** with *n* variables of width *k* and length *m* consists of a sequence of *m* instructions.
  * Each of the instructions is a tuple ( *i* ,  *p* ,  *q* ) where *i* is the index of variable to check (1 ≤ *i* ≤  *n* ), and *p* and *q* are functions from {1, 2, ...,  *k* } to {1, 2, ...,  *k* }.
  * Numbers 1, 2, ..., *k* are called states of the branching program.
  * The program initially starts in state 1, and each instruction ( *i* ,  *p* ,  *q* ) changes the state from $x$ to  $p(x)$ or  $q(x)$, depending on whether the *i*th variable is 0 or 1.
  * The function mapping an input to a final state of the program is called the *yield* of the program (more precisely, the yield on an input is the function mapping any initial state to the corresponding final state).
  * The program *accepts* a set $A\subset 2^n$ of variable values when there is some set of functions $F\subset k^k$ such that a variable sequence $x\in 2^n$ is in *A* precisely when its yield is in $F$.
* A family of branching programs consists of a branching program with *n* variables for each *n*. It accepts a language when the *n* variable program accepts the language restricted to length *n* inputs.
* Every regular language on {0,1} can be recognized by a family of branching programs of constant width and linear number of instructions (since a DFA can be converted to a branching program). **BWBP** denotes the class of languages recognizable by a family of branching programs of bounded width and polynomial length.

# Barrington's theorem

Intuition: equivalence between constant-width branching programs and logarithmic-depth circuits.

Formal statement: A language $L$ can be decided by a family of branching programs of constant width (specifically, width 5) and polynomial length if and only if $L$ is in the non-uniform complexity class $NC^1$. In other words, a branching program of width $k = 5$ can  compute any function in $NC^1$, provided its length $m$ is allowed to grow polynomially with the input size $n$.

# Proof

Sketch: The branching program is viewed as a sequence of **permutations** (elements of the symmetric group $S_5$). The final output of the program for a given input is the product of all these permutations. The non-solvability of $S_5$ provides the necessary algebraic structure to encode logical operations within the constrained memory limits of a width-5 branching program.

# Applications to Cryptography

(still looking for cool stuff) 
