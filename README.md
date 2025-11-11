<!---
{
  "id": "4b957490-badf-4264-b9f2-1b5aa370f36e",
  "teaches": "K-Map Minimization of Boolean Expressions",
  "depends_on": ["9a437897-663d-442b-82bd-f34643db7e4e"],
  "author": "Stephan Bökelmann",
  "first_used": "2025-04-01",
  "keywords": ["karnaugh map", "truth table", "boolean", "minimization"]
}
--->

# K-Map Minimization of Boolean Expressions

## 1) Introduction

Karnaugh Maps (K-Maps) provide a visual method for simplifying Boolean expressions. They allow us to group together adjacent minterms in a truth table to find minimal representations of logical functions. This becomes especially helpful in digital circuit design, where simpler expressions reduce gate count and complexity.

In this exercise, you will:

- Convert a truth table into a Karnaugh Map.
- Identify and mark groups (1s and don’t-cares) for minimization.
- Derive simplified Boolean expressions.
- Practice both single-output and multi-output scenarios.

## 2) Tasks

### Task 1: Interpreting a 3-variable K-Map

You are given the following truth table visualized in a K-Map:

|       | A=0 C=0 | A=0 C=1 | A=1 C=1 | A=1 C=0 |
|-------|---------|---------|---------|---------|
| B=0   |    1    |   0     |   1     |   1     |
| B=1   |    1    |   1     |   0     |   1     |

- Transfer this table into a 3-variable K-Map.
- Identify all groups of 1s that can be combined (groups of 1, 2, or 4).
- Derive the minimized Boolean expression.

### Task 2: Multi-output Truth Table

Based on the following truth table:

| B₁ | B₀ | A₁ | A₀ | Q₂ | Q₁ | Q₀ |
|------|------|------|------|------|------|------|
|  0   |  0   |  0   |  0   |  0   |  0   |  0   |
|  0   |  0   |  0   |  1   |  0   |  0   |  1   |
|  0   |  0   |  1   |  0   |  0   |  1   |  0   |
|  0   |  0   |  1   |  1   |  0   |  1   |  1   |
|  0   |  1   |  0   |  0   |  1   |  0   |  0   |
|  0   |  1   |  0   |  1   |  1   |  0   |  1   |
|  0   |  1   |  1   |  0   |  1   |  1   |  0   |
|  0   |  1   |  1   |  1   |  1   |  1   |  1   |
|  1   |  0   |  0   |  0   |  0   |  0   |  0   |
|  1   |  0   |  0   |  1   |  0   |  0   |  1   |
|  1   |  0   |  1   |  0   |  0   |  1   |  0   |
|  1   |  0   |  1   |  1   |  0   |  1   |  1   |
|  1   |  1   |  0   |  0   |  1   |  0   |  0   |
|  1   |  1   |  0   |  1   |  1   |  0   |  1   |
|  1   |  1   |  1   |  0   |  1   |  1   |  0   |
|  1   |  1   |  1   |  1   |  1   |  1   |  1   |

- Choose one output (e.g., Q₀) and construct a 4-variable K-Map.
- Minimize the Boolean function using grouping.
- Repeat for Q₁ and Q₂ (optional).

## 3) Questions

- What are the advantages of using a Karnaugh Map instead of algebraic simplification?
- How many cells does a K-Map need for a function with 3 inputs? What about 4 inputs?
- Why is a "gray code" ordering used in K-Maps?
- Which outputs in the second table result in the most compact logic expressions?
- What is the largest grouping (by number of 1s) you were able to make?

## 4) Advice

K-Maps help you build intuition about how logic can be minimized graphically. Always look for symmetry and adjacency in the 1s. Overlapping groups are allowed and often helpful. For multi-output circuits, look for shared logic between outputs to optimize hardware further.
