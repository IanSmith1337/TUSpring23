
#testing 

# Control Flow [[Graph]]

## Definition

A control flow [[graph]] (or flow [[graph]]) G is defined as a finite set N of [[nodes]] and a finite set E of [[edges]]. An [[edges|edge]] (i, j) in E connects two [[nodes]] ni and nj in N. We often write G= (N, E) to denote a flow [[graph]] G with [[nodes]] given by N and [[edges]] by E.

In a flow graph of a program, each [[basic block]] becomes a [[node]] and [[edges]] are used to indicate the flow of control between blocks.

## Exercise

					 (1) - If A=10
				 True |
		True	        (2) - IF B>C    False
		|--------------|-------------------|
	   (3) - A=B                  (4) - A = C

$$M= 3 - 4 + 2(3) =3-4+6 = 7 $$

Max tests: 7. 3 for variables, 4 for each edge.