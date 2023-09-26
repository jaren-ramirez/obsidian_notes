---
tags:
  - regular_expression
  - language
  - computer_science
title: automata lecture 6
Lecturer: Dr. Sebastian Neumayer
Class Number:
---
[[class_goes_here]]
```dataviewjs

```
```dataviewjs
let page = dv.current().file;
let creationTime = page.ctime;
let formattedDate = new Date(creationTime).toLocaleDateString();
dv.el("p", 'Created on ' + formattedDate)
```
# [[Regular Expression]]

## Important Links and Slides

[Link1]()
[Link2]()
## Outline

- Sub-Point
- Sub-Point
## Goals

- Clear understanding of [topic]
- Ability to explain [concept]
- Mastery of [skill/tool]
## Notes

- #### Decision Properties
	- **Finiteness: Is L a finite language**
		- DFA method
			- Given a DFA for L eleminate all states that are not reachable from the start state and all states that do not reach an accepting state
			- Test if there are any cycle in the remaining DFA if so L is infinite if not L is finite
			- Can use [[Depth First Search]] to check if a infiinte language
	- **Equivalence:**
		- Do two descriptions of a language acutally describe the same language?
			- For example two different regular expression that describe the same language
		- **Algorithm to Discover Distinguishable Pairs**
			1. Given an automaton A that has states $q_{0}...Q_n$
				- make a diagonal table with labes 1 to n on the rows and 0 to n - 1 on the columns
			2. Initialize the table by placing X's for each pair that we know is distinguishable.
				- initially this is any pair of accepting and not accepting states

   
## Questions and Clarifications

## Summary





