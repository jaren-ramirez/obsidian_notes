---
Date: 2023-09-27T11:32:00
Time: 
Lecturer: 
Topic: 
Related Textbook Chapters:
---


# Lecture Notes: [[Automata, Algorithms, and Complexity]]


## Objectives
- [Main objective 1]
- [Main objective 2]
- [Main objective 3]

## Key Points
1. **[[Pumping Lemma]]**
   - Let L be a regular language
	   - There is an integer p(the pumping length) such taht the following holds:
		   - every string s in L with |s| >= p can be written as s = xyz such that'
			   - $y \neq \epsilon \;\; (i.e |y| \geq 1)$
			   - $|xy| \neq p$
			   - $xy^{i}z \in L\:\;\; for\: all\: i \:\geq 0$
	   - Use pumping Lemma to show that this is not regular
		   - $L= \{0^{n}1^{n}\: | \: n \geq 0\}$
			   - Intuitively if you cant build a dfa for it
		   - Assume that L is regular
			   - let p be the pumping length
			   - choose $s = 0^{p}1^{p}$
		   - $L = \{w\: |\: w\: has\: an\: equal\: number\: of\: 0's\: and\: 1's \}$
		   - Assume that L is regular and let p be the pumping length
		   - Chose $s=(01)^p$
			   - s is clearly in L and $|s|\geq p$
			   - split the string into an x, y, and z subject to the pumping lemma constraints
			   - Split into $x=\epsilon$, $y=01$, and $z=(01)^{p-1}$
			   - no matter the choice for i, each resulting string is in the language so s can be pumped
   - Example or additional information
2. **[Key Point 2]**
   - Sub-point
   - Sub-point
   - Example or additional information
3. **[Key Point 3]**
   - Sub-point
   - Sub-point
   - Example or additional information

## Diagrams/Images
- [Link or embed diagrams/images here]

## Questions
- [Any questions that you have during the lecture]

## Additional Notes
- [Any additional information or notes]

## Post Lecture
- **Summary:** [Summarize the key points and important information from the lecture]
- **Action Items:** 
  - [Any assignments, readings, or work to be done post-lecture]
- **Additional Resources:**
  - [Links to additional resources related to the lecture]

---

### Links to Previous/Next Lecture Notes
- [[automata lecture 6]]
- [[automata lecture 8]]
- 

