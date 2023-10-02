
# Sessions

## Monday

### Morning 1: 

* 9-10:00: [Participants introduce themselves](Introductions.pptx), introduction of challenge problems.
* 10:00-10:30: break

### Morning 2:

* 10:30-11:30 Armin Biere - the Art of igniting the SAT revolution
* 11:30-12:00 Vijay Ganesh: [SAT + CAS: Kochen-Specker, Lam's Problem, Williamson Matrix]

### Afternoon 1: Topic Higher- order SAT.

* 14:00-14:30 Jie-Hong Roland Jiang [Second-order Boolean QBF]
* 14:30-15:00 Hiroshi Unno     [Modular Primal-Dual Fixpoint Logic Solving for Temporal Verification]
* 15:00-15:30 Sam Buss      [Seeking hard SAT instances for constant depth Frege] (encoding/challenge problem)

* 15:30-16:00 break 

### Afternoon 2: Encoding SAT

* 16:00-16:30 Stefan Szeider      [isomph-free SAT modulo symmetries]
* 16:30-17:00 Akihisa Yamada      [Satisfiability and Term Rewriting]
* 17:00-17:30 Tachio Terauchi     [Synthesizing regular expressions]
* 17:30-18:00 Discussion
  

Evening: Demos and social interaction.

## Tuesday

### Morning 1: Topic session on building SAT services on top of SAT solvers.
* 9-9:30: Katalin Fazekas     [IPASIR-UP]
* 9:30-10:00 Mathias Preiner  [CaDiCaL integration in cvc5]
* 10:00-10:30 Aina Niemetz   [local search word level reasoning, what's new with Bitwula]


### Morning 2: Applications of SAT

* 11:00-11:30 Soh Takehide        [CoRe Challenge 2022/2023: International Competition for Combinatorial Reconfiguration]
* 11:30-12:00  Mutsunori Banbara   [Hamiltonian Cycle Reconfiguration with Answer Set Programming]


### Afternoon 1: Topic session on encoding (part II). 


* 14:00-14:30       Kristin Rozier    [SAT based explicit LTLf satisfiability checking]
* 14:30-15:30       Marijn Heule      [The art of encoding happy endings]
* 15:30-16:00       break 


### Afternoon 2: Topic session on MaxSAT. Breakout session for collaborations.

* 16:00-16:30  Miyuki Koshimura      [MaxSAT application]
* 16:30-17:00  Masahiro Sakai        [Max-SAT benchmarks for Binary Neural Networks]
* 17:00-18:00  Discussions and Collaborations

### Evening: Social interaction.

## Wednesday

### Morning 1: Certificates, Search, and Beyond

* 9-9:45:      Jakob Nordström [A Unified proof logging system]
* 9:45-10:15   Shin-ichi Minato [The Art of Counting Graphs]

### Morning 2: 

* 11:00-11:30:	Matti Järvisalo [Incremental MaxSAT]
* 11:30-12:00	Oliver Kullmann   [Transforming QBFs Using Biclique Covers]


### Afternoon: excursion

## Thursday

* 9:00-9:30         Discussion on challenge problems
* 9:30-10:00        Nina Narodytska [Invariant generation using LLMs]
* 10:00-10:30       Roopsha Samanta  - [synthesis of recursive procedures]
* 10:30-11:00       Break
* 11:00-11:30       Nikolaj Bjorner [On Incremental inprocessing for SMT]
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
