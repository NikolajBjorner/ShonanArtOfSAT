
# Sessions

## Monday

### Morning: 

* 9-9:30: Participants introduce themselves, introduction of challenge problems, 2 tutorials.
* 9:30-10:30 Armin Biere - the Art of igniting the SAT revolution
* 10:30-11: Break
* 11-11:30 Vijay Ganesh: [SAT + CAS: Kochen-Specker, Lam's Problem, Williamson Matrix]
* 11:30-12 Sam Buss      [Seeking hard SAT instances for constant depth Frege] (encoding/challenge problem)

### Afternoon 1: Topic Higher- order SAT.

* 14:00-14:30 Jie-Hong Roland  [Second-order Boolean QBF]
* 14:30-15:00 Hiroshi Unno     [Modular Primal-Dual Fixpoint Logic Solving for Temporal Verification (POPL 2023 paper)]
* 15:00-15:30 Tachio Terauchi  [Synthesizing regular expressions]
  
* 15:30-16:00 break 

### Afternoon 2: Encoding SAT

* 16:00-16:30 Stephan Szeider     [isomph-free SAT modulo symmetries]
* 16:30-17:00 Akihisa Yamada      [Satisfiability and Term Rewriting]  
* 17:00-18:00 Discussion
  

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


* 14:00-14:30       Kristin Rozier    [SAT based explicit LTL satisfiability checking]
* 14:30-15:00       Marijn Heule      [Encoding]
* 15:00-15:30       [open]
* 15:30-16:00 break 


### Afternoon 2: Topic session on MaxSAT. Breakout session for collaborations.

* 16:00-16:30  Miyuki Koshimura      [MaxSAT application]
* 16:30-17:00  Masahiro Sakai        [Max-SAT benchmarks for Binary Neural Networks]
* 17:00-18:00  Discussions and Collaborations

### Evening: Social interaction.

## Wednesday

### Morning 1: Certificates, Search, and Beyond

* 9-9:45:      Jakob Nordstroem [A Unified proof logging system]
* 9:45-10:15   Nina Narodytska [Invariant generation using LLMs]

### Morning 2: 


* 11:00-11:30       Roopsha Samanta  - [synthesis of procedures - visa situation unclear]
* 11:30-12:00       Nikolaj Bjorner [On Incremental inprocessing for SMT]

### Afternoon: excursion

## Thursday

* 9-9:30:              
* 9:30-10:00         
* 10:00-10:30        

## Unconfirmed

* Katsumi Inoue 
* Oliver Kullmann   
* Matti Jaervisallo     
* Shin-ichi Minato 

## Cancelations
* Roopsha Samanta  - [visa situation unclear]
* Hidetomo Nabeshima  [canceled]
* Bart Selman  [canceled]

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



## Mutsunori Banbara

__Title__: Hamiltonian Cycle Reconfiguration with Answer Set Programming

__Abstract__:
The Hamiltonian cycle reconfiguration problem is defined as determining, for a given Hamiltonian cycle problem and two among its feasible solutions, whether one is reachable from another via a sequence of feasible solutions subject to certain transition constraints.  We develop an approach to solving the Hamiltonian cycle reconfiguration problem based on Answer Set Programming (ASP).  Our approach relies on a high-level ASP encoding and delegates both the grounding and solving tasks to an ASP-based solver.  To show the effectiveness of our approach, we conduct experiments on the benchmark set of Flinders Hamiltonian Cycle Project.

## Stefan Szeider

__Title__: Isomorph-Free Generation of Combinatorial Objects with SAT Modulo Symmetries

__Abstract__: SAT modulo Symmetries (SMS) is a framework for the exhaustive isomorph-free generation of combinatorial objects with a prescribed property. SMS relies on the tight integration of a CDCL SAT solver with a custom dynamic symmetry-breaking algorithm that iteratively refines an ordered partition of the generated object's elements. SMS utilizes the IPASIR-UP interface and hence can work with any solver implements this interface. SMS supports DRAT proofs for the SAT solver's reasoning and offline verification of the symmetry-breaking clauses, and thus provides an additional layer of confidence in the obtained results. This talk will discuss the basic concepts of SMS and review some recent applications on graphs, digraphs, hypergraphs, and matroids. 
Joint work with Katalin Fazekas, Markus Kichweger, Tomas Peitl, and Manfred Scheucher.
