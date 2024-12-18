---
permalink: /
geometry:
  - top=1in
  - bottom=1in
  - left=1in
  - right=1in
fontsize: 4pt
documentclass: article
markdown: kramdown
kramdown:
  input: GFM
  math_engine: mathjax
  syntax_highlighter: rouge
header-includes:
  - \usepackage{sectsty}
  - \allsectionsfont{\centering}
  - \usepackage{fancyhdr}
  - \usepackage{anyfontsize}
  - \usepackage{setspace}
  - |
    \makeatletter
    \renewcommand\normalsize{%
      \@setfontsize\normalsize{8pt}{10pt}%
      \abovedisplayskip 8pt
      \abovedisplayshortskip 4pt
      \belowdisplayshortskip 4pt
      \belowdisplayskip 8pt
      \abovedisplayskip 8pt
      \abovedisplayshortskip 4pt
      \belowdisplayshortskip 4pt
      \belowdisplayskip 8pt
    }
    \makeatother
---

# Computer Assisted Proofs

---

#### **Introduction**

Mathematics is often seen as a way to describe the universe. At its core, mathematics uses proofs to show that ideas and theorems are true. So these ideas can be further iterated upon. Over time, the way we create these proofs has changed a lot. This paper looks into computer-assisted proofs, exploring how they started, why they're important, and the debates about whether they're as valid as traditional proofs.

#### **Background on Mathematical Proofs**

Mathematical proofs are important because they show that a statement or theorem is **always** true. Historically, mathematicians create proofs by carefully reasoning through each step, starting from basic already proven principles and building to their final conclusion. This process helps show that every part of the proof is logically sound.

However, proofs do more than just confirm that something is true; they help others understand why it's true. By working through proofs, mathematicians can explore new ideas and deepen their knowledge of math. Many consider the beauty of traditional proofs to lie in their clarity and the fact that they reveal the underlying structure of the math they consist of.

#### **Emergence of Computer-Assisted Proofs**

As computers grew more popular though the 1900s mathematicians began using them to help with proofs. Computer-assisted proofs use algorithms to handle complex calculation and check many different cases that would be too time-consuming for any human to do by hand. The combination of the human mind and machine efficiency allows mathematicians to tackle problems that were previously out of reach due their size and complexity.

The idea of using computers to help with proofs started around the mid-20th century as computers became more powerful and efficient. At first computers where only used for simple calculations, but as technology advanced, so did the methods for utilizing computers in proofs. Now, there are specialized programs and proof assistants that can verify proofs and also help construct them with very minimal human input.

Computer-assisted proofs have led to some significant leaps in mathematics, solving many long-standing problems. These achievements show how powerful computational tools can be in advancing mathematical knowledge, challenging the traditional ways of creating proofs.

#### **Understanding Computer-Assisted Proofs**

A computer-assisted proof is a mathematical proof that relies on a computer program to verify certain sections of the argument. Where as traditional proofs are done entirely by hand using logical reasoning. Computer-assisted proofs use software to handle many complex calculations or check numerous cases that would be too time-consuming for humans to manage by themselves.

There are two main types of computer-assisted proofs:

1. **Fully Automated Proofs**: In fully automated proofs, the computer will attempt to prove the theorem with very little help. The mathematician simply sets up the problem, and the computer uses algorithms to find the proof without any human intervention. This can be very useful when problems that can be broken down into repetitive steps.

2. **Semi-Automated Proofs**: These proofs use a collaborative approach between humans and computers. While the computer handles specific complex calculations or verifies certain parts of the proof, mathematicians still guide the overall reasoning. This method is often used when parts of the proof need creative insights that computers are not capable of providing.

Creating computer-assisted proofs involves various methodologies and tools designed to work together seamlessly. Some of the most commonly used tools include:

- **Automated Theorem Provers**: These tools attempt to prove theorems automatically without much human input. They use algorithms to explore possible proof paths and find valid arguments. Examples include:
  - **Prover9**: An automated theorem prover for first-order and equational logic.
  - **E-Prover**: A theorem prover for first-order logic with equality.

- **Programming Languages**: Certain programming languages are designed to work closely with proof assistants and theorem provers. They help in writing the formal definitions and proofs that these tools can understand and verify. Examples include:
  - **ML**: Often used in proof assistants like HOL.
  - **Gallina**: The language used by Coq for writing proofs and definitions.

## **Comparison with Traditional Proofs**

Computer-assisted proofs offer some advantages over traditional proofs. One of the main benefits is their ability to handle very complex and large-scale problems that would be impractical to solve by hand. Computers can quickly perform calculations and check almost limitless cases, which enhances the precision and reliability of the proof.

However, there are also some differences in approach between computer-assisted and traditional proofs. Traditional proofs often rely on human intuition and creativity to find elegant and insightful arguments. Computer-assisted proofs may be more mechanical, focusing on exhaustive verification rather than creative reasoning.

Computer assistance is beneficial in situations where the proof requires checking a large or complex number of cases. For example, in the proof of the Four Color Theorem, a computer was used to check many different configurations of maps to ensure that four colors were sufficient. Without computer assistance, such a proof would have been nearly impossible to complete by hand.

## **Famous Examples of Computer-Assisted Proofs**

### The Four Color Theorem

The Four Color Theorem states that any planar map can be colored using at most four colors such that no two adjacent regions share the same color. In this case, adjacent refers to two regions sharing a boundary segment, not just a point.

This theorem was conjectured in 1852 by Francis Guthrie while trying to color a map of England. The theorem applies to abstract planar graphs and is a foundational result in graph theory.

**Role of Computer Assistance in the Proof**

Due to the difficulty of the Four Color Theorem to prove, many false starts and partial results came as a result. This theorem was proved in 1976 and was a one of a kind proof as it relied on computer assistance.

The key contributors in this proof were Kenneth Appel and Wolfgang Haken. whom were mathematicians at University of Illinois. They reduced the problem to only needing to check 1,936 "reducible configurations," cases.

The role of computers in this proof came when Appel and Haken needed to verify the reducibility of all 1,936 cases. This marked one of the first significant uses of computers to solve a mathematical theorem, sparking debates about the validity and nature of proofs. Due to the heavy reliance on computers, this raised concerns about trustworthiness since no human could feasibly verify all the computational steps by hand. 

### **The Kepler Conjecture**

The Kepler Conjecture assets that the most efficient way to pack identical spheres in three-dimensional space is in a face-centered cubic (FCC) or hexagonal close-packing (HCP) arrangement. These arrangements fill approximately 74.05% of the volume of space.

This conjecture was proposed by Johannes Kepler in 1611. It remained unproven for nearly four centuries and is a important result in the study of sphere packing.

**Role of Computer Assistance in the Proof**

In 1998, the proof was done by Thomas Hales and his graduate student Samuel Ferguson. The proof combined traditional mathematical reasoning alongside computer-assisted verification.

Hales and Ferguson were able to reduce the problem to an enormously large, but finite, number of specific cases by analyzing local sphere configurations. Additionally, they computed and verified complex inequalities related to the density of sphere arrangements. Manual verification is the traditional way of verification but it was infeasible in this case, so many software tools and algorithms were used for computations and verification.

The proof of the Kepler Conjecture consisted of over 250 pages of mathematical arguments and 3 gigabytes of computer-generated data. This makes this proof one of the most complex proofs ever done. 

As a result of this proof, skepticism followed. The proof was submitted to the journal *Annals of Mathematics* in 1998, where it underwent rigorous scrutiny. It was not until 2005 that the journal accepted the proof, however, they noted that verifying the computation components were not feasible by humans. 

To help verify every aspect of this proof, Hales launched the Flyspeck Project to formally prove this conjecture using automated theorem-proving systems. By 2014, Flyspeck completed the formal verification process. This achievement confirmed the correctness of Hales' proof.

**Results of the Kepler Conjecture Proof**

- The proof became a benchmark for computer-assisted proofs for longstanding mathematical problems.
- Many advancements were made in areas like automated theorem proving, discrete geometry and optimization, and mathematical philosophy.

### **The Classification of Finite Simple Groups (CFSG) Theorem**

The Classification of Finite Simple Groups is one of the most monumental achievements in modern mathematics. It states:
Every finite simple group belongs to one of the following families:
1. Cyclic groups of prime order.
2. Alternating groups $A_{n}$ for $n \ge 5$, the group of even permutations on $n$ elements.
3. Groups of Lie type
4. 26 sporadic groups (no correlation to any of the first three groups)

A finite simple group is a group that is finite, nontrivial, and has no normal subgroups other than the trivial group and itself. These are the building blocks of all finite groups, much like prime numbers are the building blocks of integers.

**Role of Computer Assistance in Proof**

The proof of the Classification of Finite Simple Groups spanned over 50 years and involved contributions from hundreds of mathematicians. The problem with proving the CFSG are the exhaustive case analyses which proved to be the most complex parts.

Many aspects of the proof required detailed examination of specific configurations, properties of subgroups, and representations. Computers were used to handle these cases efficiently. Algorithms implemented in computation algebra systems, like GAP and MAGMA, to verify properties of specific groups and their representations.

With the first three groups out of the way, studying sporadic groups relied heavily on computational techniques to explore subgroup structures and properties. Alongside sporadic groups, certain subgroup lattice configurations required computer assistance.

## **Are Computer-Assisted Proofs Really "Proofs"?**

The use of computers in mathematical proofs has created a lot of debate about whether these proofs are as legitimate as traditional proofs. Traditionally, a mathematical proof is a logical argument that demonstrates the validity of a theorem beyond doubt. These proofs are built step-by-step, using previously established facts. The process relies heavily on human creativity, and the ability to explain complex thoughts ideas clearly.

In the traditional view, proofs are not just about proving something is true; they're also about understanding why it is true. The simplicity of a proof are often valued because they provide deep insights into the mathematical concepts involved in the proof. Human mathematicians can spot patterns, make connections between various areas of math, and come up with new and innovative approaches to solve problems.

**Philosophical Perspectives**

Some mathematicians have different opinions on whether computer-assisted proofs should be considered true proofs. Some argue that since computers can handle large amounts of information and check various cases quickly, they make proofs easy to degust. From this perspective, computers are simply tools that extend human capabilities, like how calculators or telescopes help us in other fields.

On the other hand, some question the understanding of computer-assisted proofs. They argue that while a computer can confirm that each step of a proof is correct, it doesn't provide the same level of comprehension that a traditional proof does. This leads to debates about whether a proof needs to be fully disgustable by humans to be considered valid.

**Reliability and Verification**

One of the main problems with computer-assisted proofs is their reliability. Computers are programmed by humans, which means there is always a possibility of software bugs or hardware errors affecting the result of a proof. If there is a mistake in the computer program used for a proof, it could lead to incorrect or misleading results.

However, mathematicians have created various methods to ensure the correctness of computer-assisted proofs. This includes writing reliable software, performing independent checks and tests using different programs, and sometimes having multiple mathematicians review the proof and code. Additionally, projects like the Flyspeck Project for the Kepler Conjecture aim to verify every various part of a computer-assisted proof using different systems to minimize the risk of errors. Although errors do still remain possible.

**Acceptance within the Mathematical Community**

At first many mathematicians were skeptical about computer-assisted proofs. The reliance on machines that can't be fully checked rather than purely human reasoning made some question their accuracy. The Four Color Theorem and the Kepler Conjecture, which were both proven with computers assistance, were particularly controversial because their proofs involved checking thousands of cases that no human could verify on their own.

However, as time has passed, the mathematical community has become accepting of computer-assisted proofs. As technology has advanced and proof assistants have become more sophisticated and accurate. Many now see computer-assisted proofs as a valuable tool that complements traditional methods, especially for problems that are too complicated for manual proofs. While some debate still exists, the acceptance of computer-assisted proofs has significantly increased, and they are now considered a key part of modern mathematical research.

## **Conclusion**

Computer-assisted proofs have revolutionized mathematics by providing solutions to problems that are otherwise unfeasible by traditional methods. Some examples of where computer-assisted proofs shine are:

1. Handling complexity: Manages extensive case analyses and complex calculations
2. Advancing rigor of computer-assisted proofs: Automated theorem-proving systems allow for formal proofs to be produced to ensure accuracy of computer-assisted proofs.
3. Promotes collaboration: Computer tools allow mathematicians to connect ideas, test conjectures, and verify steps of proofs. 
4. Beyond Traditional Mathematics: Computer-assisted proofs inspire new questions and methods due to the endless possibilities of technology.

Mathematical proofs have always evolved alongside the different tools available to mathematicians. Traditional proofs are rooted in logical deduction and human understanding which highlight the ability to explain and understand a proofs truth. These proofs are not only about correctness but also about their ability to build connections between concepts. However, the complexity of modern problems, such as Four Color Theorem and Kepler's Conjecture, gave way to innovative proof techniques. These techniques involved computer-assisted proofs and formal proofs.

While computer-assisted proofs offer a type of precision humans do not, they challenge traditional notions of mathematical proof by prioritizing correctness over human comprehensibility. This shift has sparked an ongoing debate between tradition and innovation. Many mathematicians argue that proofs should be understandable and conceptually pretty which align with the typical aspects of mathematics; however, some mathematicians want to embrace innovation. They believe that new computational tools allow mathematics to explore territories that were previously impossible. The evolving nature of proof reflects mathematics as a living discipline, where tradition provides a foundation and innovation extends the boundaries of what is possible.
