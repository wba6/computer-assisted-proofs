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

**Introduction**

Mathematics is often seen as a way to describe the universe. At its core, mathematics uses proofs to show that ideas and theorems are true. So these ideas can be further iterated upon. Over time, the way we create these proofs has changed a lot. This paper looks into computer-assisted proofs, exploring how they started, why they're important, and the debates about whether they're as valid as traditional proofs.

**Background on Mathematical Proofs**

Mathematical proofs are important because they show that a statement or theorem is **always** true. Historically, mathematicians create proofs by carefully reasoning through each step, starting from basic already proven principles and building to their final conclusion. This process helps show that every part of the proof is logically sound.

However, proofs do more than just confirm that something is true; they help others understand why it's true. By working through proofs, mathematicians can explore new ideas and deepen their knowledge of math. Many consider the beauty of traditional proofs to lie in their clarity and the fact that they reveal the underlying structure of the math they consist of.

**Emergence of Computer-Assisted Proofs**

As computers grew more popular though the 1900s mathematicians began using them to help with proofs. Computer-assisted proofs use algorithms to handle complex calculation and check many different cases that would be too time-consuming for any human to do by hand. The combination of the human mind and machine efficiency allows mathematicians to tackle problems that were previously out of reach due their size and complexity.

The idea of using computers to help with proofs started around the mid-20th century as computers became more powerful and efficient. At first computers where only used for simple calculations, but as technology advanced, so did the methods for utilizing computers in proofs. Now, there are specialized programs and proof assistants that can verify proofs and also help construct them with very minimal human input.

Computer-assisted proofs have led to some significant leaps in mathematics, solving many long-standing problems. These achievements show how powerful computational tools can be in advancing mathematical knowledge, challenging the traditional ways of creating proofs.

**Understanding Computer-Assisted Proofs**

A computer-assisted proof is a type of mathematical proof that relies on computer programs to verify certain parts of the argument. Unlike traditional proofs, which are done entirely by hand using logical reasoning, computer-assisted proofs use software to handle complex calculations or check numerous cases that would be too tedious or time-consuming for humans to manage alone.

There are two main types of computer-assisted proofs:

1. **Fully Automated Proofs**: In these proofs, the computer takes on almost the entire role of proving the theorem. The mathematician sets up the problem, and the computer uses algorithms to find the proof without much human intervention. This approach is useful for problems that can be broken down into repetitive or highly structured steps.

2. **Semi-Automated Proofs**: These proofs involve a collaboration between humans and computers. While the computer handles specific calculations or verifies certain parts of the proof, mathematicians still guide the overall structure and reasoning. This method is often used when parts of the proof require creative insights that computers are not yet capable of providing.

Creating computer-assisted proofs involves various methodologies and tools designed to work together seamlessly. Some of the most commonly used tools include:

- **Automated Theorem Provers**: These tools attempt to prove theorems automatically without much human input. They use algorithms to explore possible proof paths and find valid arguments. Examples include:
  - **Prover9**: An automated theorem prover for first-order and equational logic.
  - **E-Prover**: A theorem prover for first-order logic with equality.

- **Programming Languages**: Certain programming languages are designed to work closely with proof assistants and theorem provers. They help in writing the formal definitions and proofs that these tools can understand and verify. Examples include:
  - **ML**: Often used in proof assistants like HOL.
  - **Gallina**: The language used by Coq for writing proofs and definitions.

**Comparison with Traditional Proofs**

Computer-assisted proofs offer several advantages over traditional, hand-written proofs. One of the main benefits is their ability to handle very complex and large-scale problems that would be impractical to solve manually. Computers can quickly perform extensive calculations and check countless cases, which enhances the precision and reliability of the proof.

However, there are also some differences in approach between computer-assisted and traditional proofs. Traditional proofs often rely on human intuition and creativity to find elegant and insightful arguments. In contrast, computer-assisted proofs may be more mechanical, focusing on exhaustive verification rather than creative reasoning.

Computer assistance is especially beneficial in situations where the proof requires checking a vast number of cases or performing complex computations. For example, in the proof of the Four Color Theorem, a computer was used to check many different configurations of maps to ensure that four colors were sufficient. Without computer assistance, such a proof would have been nearly impossible to complete.

**III. Famous Examples of Computer-Assisted Proofs**

  - **A. The Four Color Theorem**: The Four Color Theorem states that any planar map can be colored using at most four colors such that no two adjacent regions share the same color. In this case, adjacent refers to two regions sharing a boundary segment, not just a point.
    This 

##### The Four Color Theorem

**Overview**
The Four Color Theorem states that any planar map can be colored using at most four colors such that no two adjacent regions share the same color. In this case, adjacent refers to two regions sharing a boundary segment, not just a point.

This theorem was conjectured in 1852 by Francis Guthrie while trying to color a map of England. The theorem applies to abstract planar graphs and is a foundational result in graph theory.

**Role of Computer Assistance in the Proof**
Due to the difficulty of the Four Color Theorem to prove, many false starts and partial results came as a result. This theorem was proved in 1976 and was a one of a kind proof as it relied on computer assistance.

The key contributors in this proof were Kenneth Appel and Wolfgang Haken. whom were mathematicians at University of Illinois. They reduced the problem to only needing to check 1,936 "reducible configurations," cases.

The role of computers in this proof came when Appel and Haken needed to verify the reducibility of all 1,936 cases. This marked one of the first significant uses of computers to solve a mathematical theorem, sparking debates about the validity and nature of proofs. Due to the heavy reliance on computers, this raised concerns about trustworthiness since no human could feasibly verify all the computational steps by hand. 

**Impact on Graph Theory and Mathematics**
The Four Color Theorem has influenced the world of graph theory, some examples are:
1. Graph Coloring Problems:
	-  Deepened the study of graph coloring, with applications in scheduling, network design, and optimization
	-  Established planar graphs as a cornerstone in understanding combinatorial properties of networks
2. Computational Mathematics:
	 -  Pioneered computer-assisted proofs which led to the development of automated theorem proving and computational mathematics.
	 -  Brought about philosophical discussions about the nature of mathematical truth and the role of verification.
3. Practical Applications:
	 -  It helped practical problems involving graph coloring such as map creation, register allocation in compilers, and frequency assignment in telecommunications.


  - **B. The Kepler Conjecture**
    - Statement of the conjecture regarding sphere packing.
    - Description of Thomas Hales' computer-assisted proof.
    - Verification and subsequent developments.
  - **C. The Classification of Finite Simple Groups**
    - Explanation of the classification theorem.
    - Extent of computer assistance in handling extensive case analyses.
    - Significance in algebra.
  - **D. The Boolean Pythagorean Triples Problem**
    - Description of the problem.
    - Use of SAT solvers in the proof by Marijn Heule, Oliver Kullmann, and Victor Marek.
    - Discussion of the proof's size and verification.
  - **E. Other Notable Examples**
    - Brief mentions of additional theorems or conjectures utilizing computer assistance (e.g., Robertson–Seymour theorem, Ligocki's work on knot theory).

**IV. Are Computer-Assisted Proofs Really "Proofs"?**

  - **A. Traditional Notions of Proof in Mathematics**
    - Definitions and expectations of mathematical proofs.
    - The role of human intuition and creativity.
  - **B. Philosophical Perspectives**
    - Debates on the epistemological status of computer-assisted proofs.
    - Views from mathematicians and philosophers.
  - **C. Reliability and Verification**
    - Concerns about software bugs and hardware errors.
    - Efforts to ensure correctness (e.g., independent verifications, formal proofs).
  - **D. Acceptance within the Mathematical Community**
    - Historical skepticism and gradual acceptance.
    - Current consensus and differing opinions.

**V. Advantages and Limitations of Computer-Assisted Proofs**

  - **A. Advantages**
    - Ability to handle complex and large-scale problems.
    - Enhancing precision and reducing human error.
    - Facilitating exploration of new mathematical territories.
  - **B. Limitations**
    - Dependence on technology and potential obsolescence.
    - Challenges in understanding and interpreting proofs.
    - Accessibility issues for mathematicians without programming expertise.
  - **C. Balancing Human and Machine Collaboration**
    - Integrating computational tools with traditional mathematical methods.
    - Future prospects for synergy between mathematicians and technology.

**VI. The Future of Computer-Assisted Proofs**

  - **A. Technological Advancements**
    - Improvements in computing power and algorithms.
    - Emerging tools and platforms for proof verification.
  - **B. Integration with Artificial Intelligence**
    - Potential for AI to contribute to theorem discovery and proof construction.
    - Ethical and practical considerations.
  - **C. Evolving Standards and Practices**
    - Developing best practices for creating and validating computer-assisted proofs.
    - Educational implications for training future mathematicians.

**VII. Conclusion**

  - **A. Summary of Key Points**
    - Recap of the role and examples of computer-assisted proofs.
    - Overview of the debate on their validity as proofs.
  - **B. Reflection on Their Impact**
    - Influence on the advancement of mathematics.
    - Shifts in the landscape of mathematical research and proof strategies.
  - **C. Final Thoughts**
    - The evolving nature of mathematical proof.
    - The ongoing dialogue between tradition and innovation in mathematics.
