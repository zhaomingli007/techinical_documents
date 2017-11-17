	## Imperative programming vs Functional programming

1. Imperative programming
	- Modify mutable variables
	- Use assignments
	- Using control structures such as loops, break, continue and return.
	- Imperative Programs and Computers
		- Scaling up issue: limited by "Von Neumann" bottleneck  
			- Tends to conceptualize data structures **word by word** 
			<img src="https://raw.githubusercontent.com/zhaomingli007/techinical_documents/master/resources/images/Von_Neumann.png" alt="Von_Neumann architecture" style="width: 200px;"/>
			- Need to define high level abstractions such as collections, polynomials, geometric shapes, string and document.
	- Consequences for imperative programming: 
		- Theory do not admit for mutation. Such as Java string, "hello"+"world" will create a object other than modify in place
2. Functional programming
	- **Restricted** sense: Does not have mutable variables, assignments or imperative control structures. (Pule Lisp, XQuery)
	- Wider sense: focuses on functions. (Scala, Clojure, Ruby)
	- Function are first-class citizens in FP
		- Can be defined anywhere
		- Can be parameters and return as results
			