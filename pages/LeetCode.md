- [[What I Learned]]
	- [[Question]]:
	  collapsed:: true
		- Remove All Adjacent Duplicates in String II
		- You are given a string s and an integer k, a k duplicate removal consists of choosing k adjacent and equal letters from s and removing them, causing the left and the right side of the deleted substring to concatenate together.
	- how to use Pair class in [[Java]] .
	- Stack<Pair<Character, Integer>> st = new Stack<>();
	- this statement created a stack with key and value pair.
	- [[Approach]]
	  collapsed:: true
		- it would be easy if hashmaps could be applied
		- but stack cannot have multiple arguments so i created pair class
		- Pair has two arguments for this. first can be retrieved using st.getKey()
		- second the integer with st.getValue()
		-
		- [RemoveAllAdjacentDuplicatesInString2.java](../assets/RemoveAllAdjacentDuplicatesInString2_1651832115033_0.java)