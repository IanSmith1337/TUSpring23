#testing 

# Practice

1 (init) -> 2 (if x != 0) -(true)-> 3 (z=z+y) -
			|							  |
			(false)-> 4 (else z=z-y) -> 5 (y != 0) (true)-> 6(z=z/x) 
											|				      |
											(false)-> 7 (z=z\*x) -> 8

1: def(x, y, z)
2: use(x)
3: def(z), use(y)
4: z, y
5: y
6: z, x
7: z, x
8: z