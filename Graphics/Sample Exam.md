# Sample Exam

## 1.1

P0, P1, and P3 are the same.  
(Divide (x, y, z) by w).  
P2 is differing.

## P0

$$\begin{pmatrix}  3\\ 4\\ 2\\ 0.5 \end{pmatrix} = \begin{pmatrix} 3/0.5\\ 4/0.5\\ 2/0.5\\ 0.5/0.5 \end{pmatrix} = \begin{pmatrix}  6\\ 8\\ 4\\ 1 \end{pmatrix}$$

## P1

$$\begin{pmatrix}  24\\ 32\\ 16\\ 4 \end{pmatrix} = \begin{pmatrix} 24/4\\ 32/4\\ 16/4\\ 4/4 \end{pmatrix} = \begin{pmatrix}  6\\ 8\\ 4\\ 1 \end{pmatrix}$$

1.2: 

![[Pasted image 20230426153643.png]]

## Normal

$$T(d) * R(90°) * T(-c)$$

$$\begin{pmatrix}  1 & 0 & d_x\\ 0 & 1 & d_y\\ 0& 0 & 1 \end{pmatrix} * \begin{pmatrix}   cos(90°) & -sin(90°) & 0\\   sin(90°) & cos(90°)  & 0\\ 0 & 0 & 1\end{pmatrix} * \begin{pmatrix}  1 & 0 & -(c_x)\\ 0 & 1 & -(c_y)\\ 0& 0 & 1 \end{pmatrix}$$

## Inverse

$$T(-c) * R(90) * T(d)$$

$$\begin{pmatrix}  1 & 0 & -(c_x)\\ 0 & 1 & -(c_y)\\ 0& 0 & 1 \end{pmatrix} * \begin{pmatrix}   cos(90°) & -sin(90°) & 0\\   sin(90°) & cos(90°)  & 0\\ 0 & 0 & 1\end{pmatrix} * \begin{pmatrix}  1 & 0 & d_x\\ 0 & 1 & d_y\\ 0& 0 & 1 \end{pmatrix} $$

## 2.1

Determines if a point is within a triangle. 

Position of the point:

$$P=uA+vB+wC$$  

u, v, w coordinates:

$$ \begin{array}{l}
u = {\dfrac{TriangleCAP_{Area}}{TriangleABC_{Area}}}\\
v = {\dfrac{TriangleABP_{Area}}{TriangleABC_{Area}}}\\
w ={\dfrac{TriangleBCP_{Area}}{TriangleABC_{Area}}}\\
\end{array}
$$

![[Pasted image 20230426160139.png]]


3 parts of CG that use this: Color, Shading, Texture Mapping.

## 2.2

Painters algorithm can have unresolved depth order with overlapping objects 

![[Pasted image 20230426155704.png]]

Z-Buffer fixes this by checking each pixel and storing the current minimum z-value (which is closest to the camera).

![[Pasted image 20230426155743.png]]

## 3.1

![[Pasted image 20230426161317.png]]

![[Pasted image 20230426161709.png]]

![[Pasted image 20230426161337.png]]

![[Pasted image 20230426161412.png]]

![[Pasted image 20230426161432.png]]

![[Pasted image 20230426161158.png]]

## 3.2

![[Pasted image 20230426162007.png]]

![[Pasted image 20230426162021.png]]

![[Pasted image 20230426162034.png]]

![[Pasted image 20230426162046.png]]

![[Pasted image 20230426162321.png]]

![[Pasted image 20230426162340.png]]

![[Pasted image 20230426162621.png]]

## 4.1

![[Pasted image 20230426163005.png]]

![[Pasted image 20230426163014.png]]  

Example Degree = 4

**Count the LINE SEGMENTS**

![[Pasted image 20230426162914.png]]

![[Pasted image 20230426163239.png]]

![[Pasted image 20230426163248.png]]

![[Pasted image 20230426163259.png]]

![[Pasted image 20230426163309.png]]

![[Pasted image 20230426163320.png]]

![[Pasted image 20230426163332.png]]

![[Pasted image 20230426163343.png]]

## 4.2

![[Pasted image 20230426163808.png]]

![[Pasted image 20230426163825.png]]

4 Extraordinary

BL TR = 5

TR BR = 3

0 Non-quad.

![[Pasted image 20230426163837.png]]
