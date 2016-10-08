

### Task 3: [ 70 Points ] Multiplying Fractal Matrices
* In this task we will consider matrices in which some of the entries are guaranteed to be zeros, and the cells that may contain nonzero entries form a fractal shape. We will call them fractal matrices. We will only consider square matrices, and assume that for each such n × n matrix n will be a power of 2, i.e., n = 2k for some integer k ≥ 1. Row and column numbers will be from 0 to n − 1.  
The following two types of fractal matrices will be used.
	* **∆-Fractal**. A cell (i, j) will definitely contain a zero provided the bitwise AND of i and j is nonzero.
	* **∇-Fractal**. A cell (i, j) will definitely contain a zero provided the bitwise AND of (n − i − 1) and (n − j − 1) is nonzero.

	We will analyze running times of the three matrix multiplication algorithms we have seen in the class, namely the standard iterative algorithm, the standard recursive algorithm and Strassen’s algorithm, for computing products XY , where X is a ∆-fractal matrix and Y is either a ∆-fractal or a ∇-fractal or a standard matrix. The major question we will ask is if Strassen’s algorithm is still asymptotically faster than the other two algorithms.
1. [ 5 Points ] Draw ∆-fractal matrices of sizes 2 × 2, 4 × 4, 8 × 8 and 16 × 16, and only mark the cells that are not guaranteed to be zeros leaving all other cells empty. Do the same for ∇-fractal matrices.
2. [ 5 Points ] If X is an n × n ∆-fractal matrix and Y is an n × n standard matrix, what is the running time of the standard recursive algorithm for computing XY ?
3. [ 10 Points ] How will you modify the layout of the matrices so that the standard iterative algorithm can compute the product in part (b) within the same asymptotic time bound as the standard recursive algorithm?
4. [ 10 Points ] What will be the running time of Strassen’s algorithm for computing the product in part (b)?
5. [ 20 Points ] Repeat parts (b)–(d) assuming Y to be another n × n ∆-fractal matrix.
6. [ 20 Points ] Repeat parts (b)–(d) assuming Y to be an n × n ∇-fractal matrix

* **Solution: **
1. 