---
name: coding-homework
description: Method for programming assignments and coding tasks from a computer science course - reading the spec, building in tested steps, debugging, and explaining the result. Use for any task that involves writing, fixing, or reviewing code for coursework or a personal project.
---

# Coding assignments

The user is a computer science student. The code will usually be graded, often by an autograder, and the student has to understand and be able to explain it. A solution that works but ignores the assignment's rules, or that the student cannot follow, has failed.

## Read the assignment as a specification

Before writing code, extract from the assignment text and any provided files:

- The required language and version, and which libraries are allowed. Many assignments forbid the library function that would solve the task in one line.
- Required file names, function signatures, class names, and input and output formats. Autograders compare these exactly, including whitespace and trailing newlines.
- Stated constraints: input sizes, time or memory limits, required complexity, required algorithm or data structure.
- The worked examples. Turn each one into a test before writing the solution.

If the assignment text is not in the conversation, ask for it rather than guessing the requirements. If a provided skeleton exists, fill it in and leave its structure and signatures alone.

## Build in steps you can run

Get the smallest working version running first, then extend it one behaviour at a time, running the examples after each step. Choose the algorithm from the input bounds before coding: work out what complexity the limits allow and confirm the approach meets it.

Write at the level the course is at. Use the constructs and style the course material uses, and avoid advanced language features the student has not been taught unless they ask for them.

## Debugging

Reproduce the failure with the smallest input that triggers it. Read the full error and stack trace. State one hypothesis about the cause and test it with a print, a debugger, or an assertion before changing code. Fix the cause and rerun every earlier test. After two failed fixes, the assumption under them is wrong: re-read the spec and trace the code by hand on a tiny input.

## Before saying it is done

- Run the code. Never report code as working without having executed it; if you cannot run it, say so.
- Test the given examples, then the edges: empty input, a single element, duplicates, negative numbers and zero, the maximum size, and malformed input if the spec mentions it.
- Compare output to the expected format character by character.
- Re-read the assignment against the solution, requirement by requirement.
- Remove debug output and unused code.

## Explain it

Finish with a short explanation the student can learn from: the idea behind the approach, why it is correct, its time and space complexity, and any decision that was not obvious. Point out anything the student should be ready to justify to a grader.
