# Proof Builder

Proof Builder is a practice app where students build deductive proofs step by step: choosing a representation that covers every case, assembling proof steps in the only order that works, and stating the conclusion the steps support. It also runs parameterized number tricks that students then prove with symbols, and a create mode where students design their own constant number trick, watch its symbolic expression change live as they add operations, and write the conclusion in their own words. The standing teaching point throughout is that examples are evidence, never a proof, and a proof must cover every case.

Math 2201 Unit 7: Inductive and Deductive Reasoning (indicators 2.5, 2.6)

## How students use it

- Guided Proofs: seven parameterized proof families (the sum of two odd numbers is even, the sum of two even numbers is divisible by 2, the sum of two multiples of k is a multiple of k for k from 3 to 9, the sum of two consecutive integers is odd, the sum of three consecutive integers is divisible by 3, the product of two odd numbers is odd, and the sum of two consecutive odd numbers is divisible by 4), with the variable letters changing between rounds. Each round has three stages: pick the representation, assemble the steps from shuffled cards that include distractor steps, and pick the conclusion. Feedback names the specific error, such as a wrong representation, an example used as a proof, a step out of order, or a missing factor.
- Number Trick Proofs: the app presents a trick from one of three parameterized families. Students run it on two starting numbers of their choice, including negatives and fractions, to see the constant result, then assemble the symbolic steps in order and choose the conclusion the symbols support.
- Create Your Own Trick: students add up to seven operations from a palette while the builder view shows the current symbolic expression (for example, 3x + 12). They predict a final result, and the app checks whether x has disappeared, whether the constant matches their prediction, and whether any divide step can produce fractions for whole-number starting numbers. A trick that checks out is recorded with its steps, its symbolic line, and the conclusion the student wrote.

Completed proofs are collected on the printable Proof Record at the bottom of the page. The completed create-mode proof record is the Section 4 portfolio evidence artifact for this unit: it prints cleanly on its own, with the student's operations in order, the symbolic line, and their own conclusion.

## Technical notes

Single HTML file, no dependencies, works offline. All logic is inline in index.html, generation is seeded and reproducible, and a Node harness (harness.js) verifies the proof families, the trick families, and the create-mode evaluator against independently written mathematics. Nothing is recorded and nothing leaves the page.

GitHub topics when published: math-2201, inductive-deductive-reasoning, draft (draft removed after QA).
