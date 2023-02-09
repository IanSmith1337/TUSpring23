#graphics 

# Linear Algebra Review

## Point

Described by color, position, velocity, etc. Usually in matrix form.

## Rigid Body

With change in speed of the points of an object, the object doesn't lose its form.

## Vectors

Written as either -> A, **A**, or using starting and ending points -> AB.

Contains direction and length.

No absolute starting position.

### Normalization

Magnitude = ((A))

Unit vectors = Magnitude of 1.

### Addition

Hypotenuse = addition of -> A and -> B.

In Cartesian Coords: Just add.

### Multiplication

#### Dot (scalar)

A • B = ((A))((B))cos(theta)

cos(theta) = (A•B)/((A))((B))

For Unit Vectors:

cos(theta) = A-hat • B-hat

##### Projection

project b = k • A-hat

k = ((b->)) cos(theta)

#### Cross

A X B = -B X A

((A X B)) = ((A))((B))sin(theta)

Use right hand rule.

## Cartesian Coordinates

X and Y graph. Described as any orthogonal UNIT vector.

A= (x y)  
A^T = (x, y)  
((A)) = sqrt(x^2+y^2)

## Matrix

MxN array of numbers.

$$\begin{pmatrix}   1 & 2 & 3\\   4 & 5 & 6   \end{pmatrix}$$

### Matrix Multiplication

Uses Dot Product.

(M x N)(N x P) = (M x P)

$$\begin{pmatrix}   1 & 3\\   5 & 2\\ 0 & 4  \end{pmatrix}\begin{pmatrix}   3&6&9&4\\   2&7&8&3\end{pmatrix}=\begin{pmatrix}   9&?&33&13\\   19&44&61&26\\ 8&28&32&?\end{pmatrix}$$
