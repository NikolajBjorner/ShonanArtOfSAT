
# Sessions

## Monday

### Morning 1: 

* 9-10:00: [Participants introduce themselves](Introductions.pptx).
* 10:00-10:30: break

### Morning 2:

* 10:30-11:30 Armin Biere   __The Art of igniting the SAT revolution__
* 11:30-12:00 Vijay Ganesh: [__A SAT Solver + Computer Algebra Attack on the Minimum Kochen–Specker Problem__](./VijayGanesh Kochen Specker Full Slides.pptx)

### Afternoon 1: Topic Higher- order SAT.

* 14:00-14:30 Jie-Hong Roland Jiang __Second-order Boolean QBF__
* 14:30-15:00 Hiroshi Unno     __Modular Primal-Dual Fixpoint Logic Solving for Temporal Verification__
* 15:00-15:30 Sam Buss      __Seeking hard SAT instances for constant depth Frege__ (encoding/challenge problem)

* 15:30-16:00 break 

### Afternoon 2: Encoding SAT

* 16:00-16:30 Stefan Szeider      __isomph-free SAT modulo symmetries__
* 16:30-17:00 Akihisa Yamada      __Satisfiability and Term Rewriting__
* 17:00-17:30 Tachio Terauchi     __Synthesizing regular expressions__
* 17:30-18:00 Discussion
  

Evening: Demos and social interaction.

## Tuesday

### Morning 1: Topic session on building SAT services on top of SAT solvers.
* 9-9:30: Katalin Fazekas     __IPASIR-UP__
* 9:30-10:00 Mathias Preiner [__CaDiCaL(T): CaDiCaL as CDCL(T) Engine in cvc5__](./MathiasPreiner-slides.pdf)
* 10:00-10:30 Aina Niemetz   [__Bit-Blasting Meets Local Search in Bitwuzla__](./AinaNiemetz-slides.pdf)


### Morning 2: Applications of SAT

* 11:00-11:30  Mutsunori Banbara   [__Hamiltonian Cycle Reconfiguration with Answer Set Programming__](./MutsunoriBanbara-slides.pdf)
* 11:30-12:00 Soh Takehide        __CoRe Challenge 2022/2023: International Competition for Combinatorial Reconfiguration__


### Afternoon 1: Topic session on encoding (part II). 


* 14:00-14:30       Kristin Rozier    __SAT based explicit LTLf satisfiability checking__
* 14:30-15:10       Marijn Heule      __The art of encoding happy endings__
* 15:10-15:40       Nina Narodytska   __Invariant generation using LLMs__
* 15:40-16:00       break 


### Afternoon 2: Topic session on MaxSAT. Breakout session for collaborations.

* 16:00-16:30  Miyuki Koshimura      __MaxSAT application__
* 16:30-17:00  Masahiro Sakai        __Max-SAT benchmarks for Binary Neural Networks__
* 17:00-18:00  Discussions and Collaborations

### Evening: Social interaction.

## Wednesday

### Morning 1: Certificates, Search, and Beyond

* 9-9:45:      Jakob Nordström __A one-size-fits-all proof logging system?__
* 9:45-10:15   Shin-ichi Minato __The Art of Counting Graphs__

### Morning 2: 

* 11:00-11:30	Matti Järvisalo __Incremental MaxSAT__
* 11:30-12:00	Oliver Kullmann   __Transforming QBFs Using Biclique Covers__


### Afternoon: excursion

## Thursday

* 9:00-10:00        Discussion on challenge problems
* 10:00-10:30       Roopsha Samanta  - __synthesis of recursive procedures__
* 10:30-11:00       Break
* 11:00-11:30       Nikolaj Bjorner __On Incremental preprocessing for SMT__
* 11:30-12:00       Discussions 

# Abstracts

## Akihisa Yamada

__Title__: Satisfiability and Term Rewriting

__Abstract__: SAT and SMT are central tools in automatically proving termination of term rewrite systems (TRSs). In this talk, I would like to 1. explain the use of interactive SMT solving in my termination tool NaTT, and present ideas for further improvement, for which I am not sure how to encode as standard SMT problems.
2. investigate a DPLL(T)-like approach for "satisfiability modulo rewriting" (also called (in)feasibility). Such problems appear in termination and confluence analysis of (conditional) TRSs, but so far only expensive tree-automata-based techniques or basic syntactic techniques are known.

## Soh Takehide

__Title__: CoRe Challenge 2022/2023: International Competition for Combinatorial Reconfiguration

__Abstract__:
Combinatorial Reconfiguration is a novel algorithmic concept that provides mathematical models and analysis for "transformations over state spaces." Its appearance ranges from theory to applications.  However, its technical achievements are hard to access.  Thus, it is required to found a common infrastructure for utilizing and applying the algorithmic technology of combinatorial reconfiguration. See this website for more backgrounds.  

Combinatorial Reconfiguration Challenge (CoRe Challenge 2022/2023) is a competition aiming for practically exploring the combinatorial reconfiguration.  CoRe Challenge 2022/2023 targets the Independent Set Reconfiguration (ISR) problem. The ISR problem is one of the most well-studied reconfiguration problems. Theoretically, the problem is PSPACE-complete, which implies that there exist instances such that even a shortest reconfiguration sequence requires a super polynomial steps.


## Matti Järvisalo

__Title__:
Incremental Maximum Satisfiability: Interfaces, Solvers and Applications

__Abstract__:
Enabling incremental computations on the level of constraint optimization remains a noticeable challenge. Boolean satisfiability (SAT) solvers allow for incremental computations, which is key to efficient employment of SAT solvers iteratively for developing complex decision and optimization procedures, including maximum satisfiability (MaxSAT) solvers. However, while incremental computations have been identified to have great potential in speeding up especially so-called unsatisfiability-based MaxSAT solving, enabling incremental computations in MaxSAT has remained until very recently to most extent unexplored. In this talk, I will give an overview of recent developments in incremental MaxSAT, including an API supporting the development of incremental solvers and their applications; the new Incremental Track of MaxSAT Evaluations; current availability of  incremental MaxSAT solvers with some more details on  SAT-IP hybrid approach of implicit hitting sets implemented in iMaxHS; and a glance at recent successful applications of incremental MaxSAT solving.

## Mutsunori Banbara

__Title__: Hamiltonian Cycle Reconfiguration with Answer Set Programming

__Abstract__:
The Hamiltonian cycle reconfiguration problem is defined as determining, for a given Hamiltonian cycle problem and two among its feasible solutions, whether one is reachable from another via a sequence of feasible solutions subject to certain transition constraints.  We develop an approach to solving the Hamiltonian cycle reconfiguration problem based on Answer Set Programming (ASP).  Our approach relies on a high-level ASP encoding and delegates both the grounding and solving tasks to an ASP-based solver.  To show the effectiveness of our approach, we conduct experiments on the benchmark set of Flinders Hamiltonian Cycle Project.

## Stefan Szeider

__Title__: Isomorph-Free Generation of Combinatorial Objects with SAT Modulo Symmetries

__Abstract__: SAT modulo Symmetries (SMS) is a framework for the exhaustive isomorph-free generation of combinatorial objects with a prescribed property. SMS relies on the tight integration of a CDCL SAT solver with a custom dynamic symmetry-breaking algorithm that iteratively refines an ordered partition of the generated object's elements. SMS utilizes the IPASIR-UP interface and hence can work with any solver implements this interface. SMS supports DRAT proofs for the SAT solver's reasoning and offline verification of the symmetry-breaking clauses, and thus provides an additional layer of confidence in the obtained results. This talk will discuss the basic concepts of SMS and review some recent applications on graphs, digraphs, hypergraphs, and matroids. 
Joint work with Katalin Fazekas, Markus Kichweger, Tomas Peitl, and Manfred Scheucher.

## Hiroshi Unno

__Title__: Modular Primal-Dual Fixpoint Logic Solving for Temporal Verification

__Abstract__: We present a novel approach to deciding the validity of formulas in first-order fixpoint logic with background theories and arbitrarily nested inductive and co-inductive predicates defining least and greatest fixpoints. Our approach is constraint-based, and reduces the validity checking problem of the given first-order-fixpoint logic formula (formally, an instance in a language called µCLP) to a constraint satisfaction problem for a recently introduced predicate constraint language.

Coupled with an existing sound-and-relatively-complete solver for the constraint language, this novel reduction alone already gives a sound and relatively complete method for deciding µCLP validity, but we further improve it to a novel modular primal-dual method. The key observations are (1) µCLP is closed under complement such that each (co-)inductive predicate in the original primal instance has a corresponding (co-)inductive predicate representing its complement in the dual instance obtained by taking the standard De Morgan’s dual of the primal instance, and (2) partial solutions for (co-)inductive predicates synthesized during the constraint solving process of the primal side can be used as sound upper-bounds of the corresponding (co-)inductive predicates in the dual side, and vice versa. By solving the primal and dual problems in parallel and exchanging each others’ partial solutions as sound bounds, the two processes mutually reduce each others’ solution spaces, thus enabling rapid convergence. The approach is also modular in that the bounds are synthesized and exchanged at granularity of individual (co-)inductive predicates.

We demonstrate the utility of our novel fixpoint logic solving by encoding a wide variety of temporal verification problems in µCLP, including termination/non-termination, LTL, CTL, and even the full modal µ-calculus model checking of infinite state programs. The encodings exploit the modularity in both the program and the property by expressing each loops and (recursive) functions in the program and sub-formulas of the property as individual (possibly nested) (co-)inductive predicates. Together with our novel modular primal-dual µCLP solving, we obtain a novel approach to efficiently solving a wide range of temporal verification problems.


## Jakob Nordström

__Title__: A one-size-fits-all proof logging system?


__Abstract__: We propose a unified proof logging system for decision problems, optimization problems, model enumeration problems, and problem reformulations, and semantics for composition of such proofs. We discuss some of the challenges in designing such a proof system and the choices made to overcome them. We base our system on pseudo-Boolean reasoning with 0-1 integer linear programs, which is a superset of conjunctive normal form (CNF). This is the only proof system that can currently support all enhanced SAT solving techniques for decision problems, and the language of 0-1 linear inequalities also makes it convenient to reason about linear objective functions. However, to maintain equisatisfiability of decision problems restrictions for how contraints are deleted must be imposed, and this is also crucial to preserve the optimal value of optimization problem instances. In addition, for projected model enumeration, the use of strengthening rules such as RAT and pseudo-Boolean generalizations of RAT must be carefully restricted in order not to change the set of solutions. Finally, precise definitions are needed of what it would mean to rewrite the objective function and/or constraints of a problem instance while keeping it "the same", and what the semantics should be for proof compositions if a sequence of solvers operations on (translations of) the same problem instance and emit separate proof logs.

This is based on joint work with Bart Bogaerts, Stephan Gocht, Ciaran McCreesh, Magnus O. Myreen, Andy Oertel, and Yong Kiam Tan.

## Jie-Hong Roland Jiang

__Title__: Second-Order Quantified Boolean Logic

__Abstract__: 
Second-order quantified Boolean formulas (SOQBFs) generalize quantified Boolean formulas (QBFs) by admitting second-order quantifiers on function variables in addition to first-order quantifiers on atomic variables. Recent endeavors establish that the complexity of SOQBF satisfiability corresponds to the exponential-time hierarchy (EXPH), similar to that of QBF satisfiability corresponding to the polynomial-time hierarchy (PH). This fact reveals the succinct expression power of SOQBFs in encoding decision problems not efficiently doable by QBFs. In this paper, we investigate the second-order quantified Boolean logic with the following main results: First, we present a procedure of quantifier elimination converting SOQBFs to QBFs and a game interpretation of SOQBF semantics. Second, we devise a sound and complete refutation-proof system for SOQBF. Third, we develop an algorithm for countermodel extraction from a refutation proof. Finally, we show potential applications of SOQBFs in system design and multi-agent planning. With these advances, we anticipate practical tools for development.

## Vijay Ganesh

__Title__: A SAT Solver + Computer Algebra Attack on the Minimum Kochen–Specker Problem

__Abstract__:
Two of the most fundamental theorems in quantum foundations are the Kochen-Specker and the Conway-Kochen "Free Will" Theorems. Both these theorems rely on the existence of a finite object called the KS vector system. Despite several decades of effort by leading physicists and mathematicians, the minimum KS system problem for 3-dimensions remains unresolved. In this talk, we present a SAT solver + Computer Algebra (CAS) attack on this problem, and provide a verified computational proof that there are no KS systems of  size 23 or below. To the extent that we know, ours is the first attack on a problem in quantum foundations via a combination of a SAT solver and CAS system.


## Mathias Preiner
__Title__: CaDiCaL(T): CaDiCaL as CDCL(T) Engine in cvc5

__Abstract__:
cvc5 is a state-of-the-art SMT solver based on the CDCL(T) framework, which
tightly integrates theory solvers with a CDCL SAT solver at its core.
The CDCL(T) framework requires a tight integration with the SAT solver in a way
that allows the theory layer to interact with the SAT solver during search,
i.e., in an online fashion.
For this purpose, cvc5 integrates a heavily customized version of MiniSat 2.2.0,
which was extended to allow this online interaction.

In this talk, I will discuss the integration of CaDiCaL as CDCL(T) SAT engine in
cvc5 via the recently proposed IPASIR-UP interface. IPASIR-UP is an interface
for interactive incremental SAT solving for interacting with a CDCL SAT solver
during search. I will explain in detail how the notifications and callbacks of
IPASIR-UP are used to establish the communication between cvc5's theory solvers
and CaDiCaL and how we use it to inspect and influence the CDCL search. I will
conclude with an evaluation on SMT-LIB and discuss some challenges we
encountered on incremental SMT-LIB problems.


## Aina Niemetz
__Title__: Bit-Blasting Meets Local Search in Bitwuzla

__Abstract__:
Reasoning about quantifier-free bit-vector constraints in Satisfiability
Modulo Theories (SMT) has been an ongoing challenge for many years,
especially for large bit-widths. Current state-of-the-art for bit-precise
reasoning is a technique called bit-blasting, where bit-vector constraints
are eagerly translated into propositional logic (SAT). Bit-blasting is very
efficient in practice but does not generally scale well for large bit-widths
due to fact that the translation is in general exponential in the size of the
input formula, which potentially (and in practice) overwhelms the underlying
SAT solver. For these instances, we need alternative approaches for
bit-precise reasoning that do not rely on translations to the SAT level.
Such an alternative approach is our propagation-based local search procedure,
which relies on propagating target values from top-level constraints towards
the inputs while utilizing so-called invertibility conditions. Invertibility
conditions precisely characterize when bit-vector constraints are invertible,
a core concept of our approach. Our procedure is, as expected for local
search, incomplete in the sense that it can only determine satisfiability but
was shown to be effective on hard satisfiable instances, in particular in
combination with bit-blasting in a sequential portfolio setting. In this talk,
I will talk about the strengths and potential weaknesses of this approach,
how to address these weaknesses, and the challenge to combine local search
with bit-blasting, as implemented in our new SMT solver Bitwuzla, in a
more hybrid manner that allows information sharing between the two approaches.
