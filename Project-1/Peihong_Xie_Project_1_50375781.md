# Project 1 Assignment

Your first project will require you to answer each of the 10 questions below.  You will be expected to open a pull request with your initial answers by the second class meeting, giving you one week to work on these problems. You and your peers will then have one week to work together to refine your respective initial answers, so they are ready for final submission. Once your pull requests have been reviewed and merged to the development branch, I will review them, then merge to the master branch. 

```Tip #1: Carefully study the Hedman selections assigned, as several of the questions are taken directly from the textbook. 
Tip #2: Google is your friend. An important skill to pick up in this class is recognizing when to think hard and when to think smart. You might find answers to some of the questions below simply by googling; you might find pieces of answers to parts of some question below, which will need to be combined; then again, you might not find any help at all because the questions are more novel than they initially appear. I encourage you to use existing resources as guidance, but be careful. My reputation for asking students tricky questions is well-earned. 
Tip #3: Work _together_ to solve these problems, even for initial submissions and when you do, document this in github. For example, you might feel like you nearly have answers to question 1, but would love another pair of eyes. You can then open a post in your local github account, and tag folks from class requesting they check out your work. 
Tip #4: The work we do is challenging; that should be assumed. You are smart enough to be here; that should also be assumed. We have neither time nor space for shaming, but all of time and space for praising. Be cognizant of how your messages might be received, and err on the side of caution. It is hard to surmise intent from text alone. For my part, I treat text only communications the way modern musicals are written: Little subtext; emotions on the sleeve. 
```


Note: The standard interpretation of the logical symbols - "∨", "∧", "→", "¬", "∀", "∃" - is assumed throughout.  


[1] Provide the truth tables for each of the following propositional logic formulas. State whether each is a tautology, a contradiction, or contingent:
  ```(a) (¬A→B)∨((A∧¬C)→B) 
  (b) (A→B)∧(A→¬B)
  (c) (A→(B∨C))∨(C→¬A) 
  (d) ((A→B)∧C)∨(A∧D) 
```

Answer: 

(a) Tautology
| A | B	| C | ¬A→B | A∧¬C | (A∧¬C)→B | (¬A→B)∨((A∧¬C)→B) |
| ---  | --- | --- | --- | --- | --- | --- |
| 1 | 1 | 1 | 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 | 1 | 1 | 1 |
| 1 | 0 | 1 | 1 | 0 | 1 | 1 |
| 0 | 1 | 1 | 1 | 0 | 1 | 1 |
| 1 | 0 | 0 | 1 | 1 | 0 | 1 |
| 0 | 1 | 0 | 1 | 0 | 1 | 1 |
| 0 | 0 | 1 | 0 | 0 | 1 | 1 |
| 0 | 0 | 0 | 0 | 0 | 1 | 1 |

(b) Contingent
| A | B	| A→B | A→¬B | (A→B)∧(A→¬B) | 
| ---  | --- | --- | --- | --- |
| 1 | 1 | 1 | 0 | 0 | 
| 1 | 0 | 0 | 1 | 0 |
| 0 | 1 | 1 | 1 | 1 |
| 0 | 0 | 1 | 1 | 1 | 

(c) Tautology
| A | B	| C | B∨C | A→(B∨C) | C→¬A | (A→(B∨C))∨(C→¬A)) |
| ---  | --- | --- | --- | --- | --- | --- |
| 1 | 1 | 1 | 1 | 1 | 0 | 1 |
| 1 | 1 | 0 | 1 | 1 | 1 | 1 |
| 1 | 0 | 1 | 1 | 1 | 0 | 1 |
| 0 | 1 | 1 | 1 | 1 | 1 | 1 |
| 1 | 0 | 0 | 0 | 0 | 1 | 1 |
| 0 | 1 | 0 | 1 | 1 | 1 | 1 |
| 0 | 0 | 1 | 1 | 1 | 1 | 1 |
| 0 | 0 | 0 | 0 | 1 | 1 | 1 |

(d) Contingent
| A | B	| C | D | A→B | (A→B)∧C | A∧D | ((A→B)∧C)∨(A∧D)
| ---  | --- | --- | --- | --- | --- | --- |--- |
| 1  | 1 | 1 | 1 | 1 | 1 | 1 | 1 |
| 1  | 1 | 1 | 0 | 1 | 1 | 0 | 1 |
| 1  | 1 | 0 | 1 | 1 | 0 | 1 | 1 |
| 1  | 0 | 1 | 1 | 0 | 0 | 1 | 1 |
| 0  | 1 | 1 | 1 | 1 | 1 | 0 | 1 |
| 1  | 1 | 0 | 0 | 1 | 0 | 0 | 0 |
| 1  | 0 | 1 | 0 | 0 | 0 | 0 | 0 |
| 0  | 0 | 1 | 1 | 1 | 1 | 0 | 1 |
| 0  | 1 | 1 | 0 | 1 | 1 | 0 | 1 |
| 0  | 1 | 0 | 1 | 1 | 0 | 0 | 0 |
| 1  | 0 | 0 | 1 | 0 | 0 | 1 | 1 |
| 0  | 0 | 0 | 1 | 1 | 0 | 0 | 0 |
| 0  | 0 | 1 | 0 | 1 | 1 | 0 | 1 |
| 0  | 1 | 0 | 0 | 1 | 0 | 0 | 0 |
| 1  | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 0  | 0 | 0 | 0 | 1 | 0 | 0 | 0 |

[2] A _literal_ is an atomic formula or the negation of an atomic formula. We say a formula is in _conjunctive normal form_ (CNF) if it is the conjunction of the disjunction of literals. Find propositional logic formulas in CNF equivalent to each of the following:
  ```(a) (A→B)→C
  (b) (A→(B∨C))∨(C→¬A)
  (c) (¬A∧¬B∧C)∨(¬A∧¬C)∨(B∧C)∨A 
```
Answer:

(a) CNF: (A∨C)∧(¬B∨C)

(b) CNF: B∨¬B (the CNF of a tautology is any formula of the form "p∨¬p")

(c) CNF: B∨¬B (the CNF of a tautology is any formula of the form "p∨¬p")

[3] Let V be the vocabulary of first-order logic consisting of a binary relation P and a unary relation F. Interpret P(x,y) as “x is a parent of y” and F(x) as “x is female.” Where possible define the following formulas in this vocabulary; where not possible, explain why: 
  ```(a)  B(x,y) that says that x is a brother of y
  (b)  A(x,y) that says that x is an aunt of y
  (c)  C(x,y) that says that x and y are cousins 
  (d)  O(x) that says that x is an only child
  (e)  T(x) that says that x has exactly two brothers 
```

Answer:


(a) B(x,y) $\leftrightarrow$ ∃u(P(u,x)∧P(u,y))∧¬F(x)∧¬(x=y)

(b) A(x,y) $\leftrightarrow$ ∃u∃w(P(u,y)∧P(w,x)∧P(w,u)∧¬(x=u))∧F(x)

(c) C(x,y) $\leftrightarrow$ ∃s∃u∃v∃w∃z(P(w,z)∧P(z,x)∧((P(w,u)∧P(u,y))∨(P(s,w)∧P(s,v)∧P(v,u)∧P(u,y)))∧¬(x=y)

Here consider two situations (by disjunction):

(i) x's parent z has sibiling u (who has the same parent w as z), and y is u's child and thus x's first cousion.
(ii) x's grandparent w has sibiling v (who has the same parent s as w), and y is a grandchild of v and thus a second cousin of x. 



(d) O(x) $\leftrightarrow$ ∃u(P(u,x)∧∀y(P(u,y)→x=y))

(e) T(x) $\leftrightarrow$ ∃u∃y∃z(¬(y=z)∧¬(x=y)∧¬(x=z)∧P(u,x)∧P(u,y)∧P(u,z)∧¬F(y)∧¬F(z))∧∀w(P(u,w)∧¬F(w)→ w=x ∨ w=y ∨ w=z)



[4] Let V be a vocabulary of the attribute (concept) language with complements (ALC) consisting of a role name "parent_of" and a concept name "Male". Interpret parent_of as "x is a parent of y" and M as "x is male". Where possible define the following formulas in this vocabulary; where not possible, explain why: 
  ```(a)  B that says that x is a brother of y
  (b)  A that says that x is an aunt of y
  (c)  C that says that x and y are cousins 
  (d)  O that says that x is an only child
  (e)  T that says that x has exactly two brothers 
```

Answer:

**Given ALC has no inverse role or numerical restrictions, B, A, C, O, and T cannot be represented here. For example, a brother must be a child of someone, but he might not be a parent of someone (if he is barren). That is, without the inverse role of parent_of, it is impossible to characterize him as a brother only by using parent_of.** 

The following are some definitional attempts within ALCIN.

**Approach 1 for ALCIN (directly introducing the inverse of a primary role)**

(a) $B ≡ M\sqcap ∃parentOf^-.(\ge2 parentOf.(M\sqcup ¬M))$

(b) $A ≡ ¬M\sqcap ∃parentOf^-.((∃parentOf.(∃parentOf.M\sqcup ¬M))\sqcap \ge2 parentOf.(M\sqcup ¬M))$

(c) $C ≡ ∃parentOf^-.(∃parentOf^-.(\ge2parentOf.(∃parentOf.M\sqcup ¬M)))$

(d) $O ≡ ∃parentOf^-.(\le1 parentOf.(M\sqcup ¬M))$

(e) $T ≡ (M\sqcap ∃parentOf^-.(\le3 parentOf.M \sqcap \ge3 parentOf.M))\sqcup(¬M\sqcap∃parentOf^-.(\le2 parentOf.M \sqcap \ge2 parentOf.M))$


**Approach 2 for ALCIN (indirectly introducing the inverse of a primary role, based on Ali and Giacomo, after my revisions)**

In fact, these two approaches are interchangable because $parentOf^-$ in my own approach plays the same role as $p1^-$ in my revised Ali and Giacomo's approach:

(a) B that says that x is a brother of y

  Person ≡ M ⊔ ¬M

  **p2** (parent of at least 2 children) ≡ ≥2 ∃parent_of.Person

  The inverse of p2 means that x is one of at least 2 children produced by y.

  B (brother) ≡ M ⊓ ∃p2¯.Person

(b)  A that says that x is an aunt of y
  
  A ≡ ¬M ⊓ (∃p2¯.(≥ 2 parent_of. (∃parent_of. Person)) ⊔ ¬∃parent_of. Person)

(c)  C that says that x and y are cousins

  **gp2** (Grandparent with at least two children which each have children) ≡ ≥2 parentof. (∃parentof. Person)

  C ≡ gp2¯. Person

  But this would only describe one of the two cousins, i.e. "being a cousin of someone" or "having a cousin". We cannot define "being cousins" in description logic.

(d)  O that says that x is an only child  

  **parent_only** (be a parent of exactly one child) ≡ (≥1 parent_of. Person) ⊓ (≤1 parent_of. Person)
  
  O ≡ ∃parent_only¯.Person

(e)  T that says that x has exactly two brothers. 

  **p3m** (be a parent of exactly three male children) ≡ (≥3 parent_of. Male) ⊓ (≤3 parent_of. Male)

  **p1** (be a parent of at least one child) ≡ ≥1 parent_of. Person -- the inverse of p1 is just "be a child of"!

  T ≡ ∃p3m¯.Person ⊔ (¬M ⊓ ∃p1¯. (≥2 parent_of. Male ⊓ ≤2 parent_of. Male)) 

  -- This means, either x is one of exactly 3 boys produced by a person (so x has exactly two brothers), or x is female and is a child of a person who has exactly two boys (so x has also exactly two brothers)

[5] Select two formulas defined in ALC from question 4 to form the basis of a T-Box. Supplement this T-box with whatever other axioms you like, as well as an A-box, so that you ultimately construct a knowledge base K = (T,A). Provide a _model_ of K. This may be graphical or symbolic or both. 

Answer:

**There is no formula from Question 4 available here.**

$K_1 = (T_1,A_1)$ such that:

T-box $T_1$={GP (grandparent) ≡ ∃parentOf.(∃parentOf.M∪¬M)}

A-box $A_1$={(Mary,Karl):ParentOf, Karl:Male}.

The following is a model $\Im=(\bigtriangleup^\Im,.^\Im)$ of $K_1$:

$\bigtriangleup^\Im$={a,b,c}

$M^\Im$={a}

$GP^\Im$={c}

$parentOf^\Im$={(c,b),(b,a)}

$Karl^\Im$={a}

$Mary^\Im$={b}

$Jack^\Im$={c}

[6] Explain the difference - using natural language - between the first-order prefixes:
  ```(a) ∃x∀y and ∀x∃y
  (b) ∃x∀y∃z and ∀x∃y∀z 
  (c) ∀x∃y∀z∃w and ∃x∀y∃z∀w
```
Answer:

(a) ∃x∀y means “there exists x such that for all y” while ∀x∃y means "for all x, there exists y such that"

(b) ∃x∀y∃z means “there exists x such that for all y, there exists z such that” while ∀x∃y∀z means "for all x, there exists y such that for all z"

(c) ∀x∃y∀z∃w means "for all x, there exists y such that for all z, there exists w such that" while ∃x∀y∃z∀w means "there exists x such that for all y, there exists z such that for all w"

[7] Show that the following sentences are not equivalent by exhibiting a graph that models one but not both of these sentences:
```
∀x∃y∀z(R(x,y) ∧ R(x,z) ∧ R(y,z))
∃x∀y∃z(R(x,y) ∧ R(x,z) ∧ R(y,z))
```

Answer:

The following graph models the second sentence but not the first sentence:

Verticles: a, b, c

Edges: ab, ac, aa (loop)

```mermaid
graph LR
A((a)) ---B((b))
A((a)) ---C((c))
A((a)) ---A((a))
```
	
[8] Using an online tableau proof generator - such as the one found here `https://www.umsu.de/trees/` - provide tree proofs of the following entailments, which are known as the De Morgan's laws:
```
(a) ∀x∀y(¬(Px ∧ Qx) → (¬Px ∨ ¬Qx))
(b) ∀x∀y(¬(Px ∨ Qx) → (¬Px ∧ ¬Qx))
(c) ∀x∀y((¬Px ∨ ¬Qx) → ¬(Px ∧ Qx))
(d) ∀x∀y((¬Px ∧ ¬Qx) → ¬(Px ∨ Qx))
```

Answer:

(a)

![picture 1](https://github.com/peihongx/PHI-696/blob/main/Project-1/tree_1.jpg)

(b)(c)

![picture 2](https://github.com/peihongx/PHI-696/blob/main/Project-1/tree_2.jpg)  


(d)

![picture 3](https://github.com/peihongx/PHI-696/blob/main/Project-1/tree_3.jpg)


[9] Using a natural deduction proof generator - such as the one found here `https://proofs.openlogicproject.org/` - provide natural deduction proofs for each of De Morgan's laws. 

Answer:

(a) 

![picture 1](https://github.com/peihongx/PHI-696/blob/main/Project-1/fitch_proof_1.PNG) 

(b) 

![picture 1](https://github.com/peihongx/PHI-696/blob/main/Project-1/fitch_proof_2.PNG) 

(c) 

![picture 1](https://github.com/peihongx/PHI-696/blob/main/Project-1/fitch_proof_3.PNG) 

(d) 

![picture 1](https://github.com/peihongx/PHI-696/blob/main/Project-1/fitch_proof_4.PNG) 

[10]   Compare and contrast the proofs provided for (a) in your answers to questions 8 and 9. Explain the different assumptions, strategies, etc. exhibited in tree proofs vs natural deduction proofs. 

Answer: 

For (a), a Fitch-style natural deduction proof relies on deductive rules like disjunction elimination or double negation elimination (DNE) to a more substantive degree than a tree proof. 

While a Fitch-style natural deduction proof is a **combinational application of different means of derivation**, a tree proof is essentially **an application of indirect derivation**. That is, when we do a tree proof, we have to decompose the target (complex) formula into its subformulas, and then differently connect negations of those subformulas in order to form different paths. Once when all paths somehow involve a contradiction, then the opposite possibilities of the target formula are all shown to be implausible, and thus the target formula will be proved.

Moreover, a Fitch-style natural deduction proof is to apply rules to the target formula and its logical consequents, while a tree proof does not apply the same rules but concentrates on finding possible logical contradictions among negated subformulas of the target formula. 
