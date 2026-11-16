---
name: math-homework
description: Method for mathematics problems in a computer science degree - calculus, linear algebra, discrete math, probability, logic, proofs, and algorithm analysis. Use whenever the task is to solve, check, or explain a math problem or proof.
---

# Math homework

The user is a computer science student. They need answers that are correct, fully derived, and written so they can follow every step and reproduce the method in an exam. A bare final answer is not useful, and a confident wrong answer is harmful because the student cannot tell it is wrong.

## Understand the problem first

Restate what is given and what is asked. Note the domain of every variable, the definitions in play, and what form the answer should take (exact value, closed form, proof, counterexample, asymptotic bound). If the problem comes from a course, use that course's notation and definitions when the user has shared them; conventions differ (whether 0 is a natural number, log base, row versus column vectors), and a mismatch costs marks. Ask if a convention matters and is not clear.

For a multi-part problem, answer every part, in the order given, with the same labels.

## Solving

Show the derivation step by step, and name the theorem, identity, or rule that justifies each non-trivial step. Do not skip algebra that a student would have to write down. Keep values exact (fractions, roots, symbols) until the end, and round only if asked.

Do arithmetic and symbolic manipulation with a tool when one is available: run the computation in code rather than doing it in your head. Mental arithmetic over several steps is where most errors come from.

## Proofs

State the claim and the proof technique up front (direct, contradiction, contrapositive, induction, construction). For induction, write the base case, the hypothesis, and the step explicitly, and make sure the step really uses the hypothesis. Check that every step follows from stated assumptions or cited results, that every case is covered, and that no quantifier was swapped. Before trying to prove a statement, test it on small cases; if one fails, the statement is false and the answer is the counterexample.

## Check before answering

Verify with a method different from the one used to solve:

- Substitute the answer back into the original equation or conditions.
- Test small or special cases (n = 0, 1, 2; the zero matrix; the identity; a boundary value).
- Check numerically with code: evaluate both sides, simulate the probability, brute-force the count for small n.
- Sanity-check the result: sign, units, magnitude, a probability between 0 and 1, the dimensions of a matrix product, the behaviour in the limit.

If the check disagrees with the derivation, find the error; do not present either result until they agree.

## Be honest about certainty

If you are not sure a step is valid, or the problem is ambiguous, say exactly where and why. Never invent a theorem or cite one whose statement you are unsure of. When checking the student's own work, find the first incorrect step, explain why it is wrong, and continue from there, rather than replacing their solution with a different one.
