# Sample Exam

## 1.1 Homogeneous Coordinates

P0, P1, and P3 are the same.  
(Divide (x, y, z) by w).  
P2 is differing.

## P0

$$\begin{pmatrix}  3\\ 4\\ 2\\ 0.5 \end{pmatrix} = \begin{pmatrix} 3/0.5\\ 4/0.5\\ 2/0.5\\ 0.5/0.5 \end{pmatrix} = \begin{pmatrix}  6\\ 8\\ 4\\ 1 \end{pmatrix}$$

## P1

$$\begin{pmatrix}  24\\ 32\\ 16\\ 4 \end{pmatrix} = \begin{pmatrix} 24/4\\ 32/4\\ 16/4\\ 4/4 \end{pmatrix} = \begin{pmatrix}  6\\ 8\\ 4\\ 1 \end{pmatrix}$$

## 1.2 Transforms

![[Pasted image 20230426153643.png]]

## Normal

$$T(d) * R(90°) * T(-c)$$

$$\begin{pmatrix}  1 & 0 & d_x\\ 0 & 1 & d_y\\ 0& 0 & 1 \end{pmatrix} * \begin{pmatrix}   cos(90°) & -sin(90°) & 0\\   sin(90°) & cos(90°)  & 0\\ 0 & 0 & 1\end{pmatrix} * \begin{pmatrix}  1 & 0 & -(c_x)\\ 0 & 1 & -(c_y)\\ 0& 0 & 1 \end{pmatrix}$$

## Inverse

$$T(-c) * R(90) * T(d)$$

$$\begin{pmatrix}  1 & 0 & -(c_x)\\ 0 & 1 & -(c_y)\\ 0& 0 & 1 \end{pmatrix} * \begin{pmatrix}   cos(90°) & -sin(90°) & 0\\   sin(90°) & cos(90°)  & 0\\ 0 & 0 & 1\end{pmatrix} * \begin{pmatrix}  1 & 0 & d_x\\ 0 & 1 & d_y\\ 0& 0 & 1 \end{pmatrix} $$

## 2.1 Barycentric Coordinates

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

## 2.2 Painters and Z-Buffer

Painters algorithm can have unresolved depth order with overlapping objects 

![[Pasted image 20230426155704.png]]

Z-Buffer fixes this by checking each pixel and storing the current minimum z-value (which is closest to the camera).

![[Pasted image 20230426155743.png]]

## 3.1 Shading and Blinn-Phong

![[Pasted image 20230426161317.png]]

![[Pasted image 20230426172614.png]]

![[Pasted image 20230426161709.png]]

![[Pasted image 20230426161337.png]]

![[Pasted image 20230426161412.png]]

![[Pasted image 20230426161432.png]]

![[Pasted image 20230426161158.png]]

## 3.2 Artifacts and Texture Anti-aliasing

![[Pasted image 20230426162007.png]]

![[Pasted image 20230426162021.png]]

![[Pasted image 20230426162034.png]]

![[Pasted image 20230426162046.png]]

![[Pasted image 20230426162321.png]]

![[Pasted image 20230426162340.png]]

![[Pasted image 20230426162621.png]]

## 4.1 Bezier Curves

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

## 4.2 Catmull-Clark Subdivision

![[Pasted image 20230426163808.png]]

![[Pasted image 20230426163825.png]]

4 extraordinary.

BL TR = 5

TR BR = 3

All quadfaces.

![[Pasted image 20230426163837.png]]

![[ExtrodrinaryMesh.jpg]]

# Extra Topics

# Dot Product

![[Pasted image 20230426171108.png]]

# Cross Product

![[Pasted image 20230426171200.png]]

# 2D Transformation

## Scale

S(x, y):

$$ 
x' = sx
$$

$$ 
y' = sy
$$

$$\begin{pmatrix}   x'\\   y'   \end{pmatrix} = \begin{pmatrix}   s_x & 0\\   0 & s_y  \end{pmatrix} \begin{pmatrix}   x\\   y   \end{pmatrix}
$$

## Reflection

Horizontal: 

$$ 
x' = -x
$$

$$ 
y' = y
$$

Vertical: 

$$ 
x' = x
$$

$$ 
y' = -y
$$

Reflection Matrix (x):

$$\begin{pmatrix}   x'\\   y'   \end{pmatrix} = \begin{pmatrix}   -1 & 0\\   0 & 1  \end{pmatrix} \begin{pmatrix}   x\\   y   \end{pmatrix}
$$

Reflection Matrix (y):

$$\begin{pmatrix}   x'\\   y'   \end{pmatrix} = \begin{pmatrix}   1 & 0\\   0 & -1  \end{pmatrix} \begin{pmatrix}   x\\   y   \end{pmatrix}
$$

## Shear

Horizontal shear:

$$\begin{pmatrix}   x'\\   y'   \end{pmatrix} = \begin{pmatrix}   1 & a\\   0 & 1  \end{pmatrix} \begin{pmatrix}   x\\   y   \end{pmatrix}
$$

Vertical shear:

$$\begin{pmatrix}   x'\\   y'   \end{pmatrix} = \begin{pmatrix}   1 & 0\\   a & 1  \end{pmatrix} \begin{pmatrix}   x\\   y   \end{pmatrix}
$$

## Rotation (about origin)

CCW:

$$r(\theta):$$

$$ R_\theta = \begin{pmatrix}   cos(\theta) & -sin(\theta)\\   sin(\theta) & cos(\theta)  \end{pmatrix}
$$

CW: 

$$r(-\theta):$$

$$ R_{-\theta} = \begin{pmatrix}   cos(-\theta) & -sin(-\theta)\\   sin(-\theta) & cos(-\theta)  \end{pmatrix} = \begin{pmatrix}   cos(\theta) & sin(\theta)\\   -sin(\theta) & cos(\theta)  \end{pmatrix}
$$

## Translation

$$ 
x' = t_x + x
$$

$$ 
y' = t_y+y
$$

## Affine

![[Pasted image 20230426172350.png]]

## Inverse

Basically undoes a transform.

## Composite Transform

Order of transform matters. 

## Composing Transforms

A sequence of Affine Transforms, composed by matrix multiplication.

## Rotation around a Certain point (not origin)

3 steps:

1. Translate to origin
2. Rotate
3. Translate back.  

$$T(c) * R(\alpha) * T(-c)$$

**NOTE: REVERSE ORDER ABOVE IS ON PURPOSE!**

# 3D Transformation

## Scale

$$ S = \begin{pmatrix}   S_x & 0 & 0 & 0\\ 0 & S_y & 0 & 0\\   0 & 0 & S_z & 0\\ 0 & 0 & 0 & 1  \end{pmatrix}
$$

## Translation

$$ T = \begin{pmatrix}   1 & 0 & 0 & T_x\\ 0 & 1 & 0 & T_y\\   0 & 0 & 1 & T_z\\ 0 & 0 & 0 & 1  \end{pmatrix}
$$

## Rotation (about origin)

$$ R_x(\alpha) = \begin{pmatrix}   1 & 0 & 0 & 0\\ 0 & cos(\alpha) & -sin(\alpha) & 0\\   0 & sin(\alpha) & cos(\alpha) & 0\\ 0 & 0 & 0 & 1  \end{pmatrix}
$$

$$ R_y(\alpha) = \begin{pmatrix}   cos(\alpha) & 0 & sin(\alpha) & 0\\ 0 & 1 & 0 & 0\\   -sin(\alpha) & 0 & cos(\alpha) & 0\\ 0 & 0 & 0 & 1  \end{pmatrix}
$$

$$ R_z(\alpha) = \begin{pmatrix}   cos(\alpha) & -sin(\alpha) & 0 & 0\\ sin(\alpha) & cos(\alpha) & 0 & 0\\ 0 & 0 & 1 & 0\\ 0 & 0 & 0 & 1  \end{pmatrix}
$$

# Homogeneous Coordinates

## Usage

Used in 2D Transformation.

## Method for Translation

Add a third coordinate (with value 1 for point, 0 for vector), then create matrix.

$$\begin{pmatrix}   x'\\   y'\\ w'   \end{pmatrix} = \begin{pmatrix}   1 & 0 & t_x\\   0 & 1 & t_y \\ 0 & 0 & 1 \end{pmatrix} \begin{pmatrix}   x\\   y\\  1   \end{pmatrix}
$$

## Valid Ops

Vector + Vector = Vector

Point - Point = Vector

Point + Vector = Point

Point + Point = ??

## Details

$$\begin{pmatrix}   x\\   y\\ w   \end{pmatrix}$$  

is the 2D Point

$$\begin{pmatrix}   x/w\\   y/w\\ 1   \end{pmatrix}$$

when w ≠ 0

# Perspective Projection Matrix

![[Pasted image 20230426171418.png]]

# Orthographic Matrix

## Definition

Camera at origin (-Z look, Y up)

Drops Z coordinate

## Finding Center

$$\frac{l+r}{2}, \frac{t+b}{2}, \frac{f+n}{2}$$

## Final Matrix

![[Pasted image 20230426171542.png]]

# MVP

~~most valuable person~~

![[Pasted image 20230426172158.png]]

# Rasterization

## Definition

The fragmentation of shapes and primitives into [[Pixel|pixels]]. Rasterizing is drawing to a [[Raster]], aka [[Screen]].

# Sampling

## Definition

Nothing in [[Computer Graphics]] is continuous. Sampling determines if a [[Pixel]] has a certain value on a [[Screen]]. Implementation of [[Rasterization]].

## Types

[[Bounding Box]]  
[[Incremental Triangle Traversal]]

## Using Cross Products to Determine Interior

Using p0 and p1 (two points of triangle) then drawing a line from p0 to the point to evaluate: if cross product shows that the point is in the direction of interior and overlapping on all three sides of triangle, then it is inside.

# Bounding Box

## Definition

bottom-left: Min_x(x1, x2, x3), min_y(y1, y2, y3)

top-right: max_x(x1, x2, x3), max_y(y1, y2, y3)

# Incremental Triangle Traversal

## Method

Move right as far as possible, then move up one pixel from leftmost point still inside of triangle.

# [[Shading]] Frequencies

## Definition

How many samples should be taken for each tri.

![[Pasted image 20230426172708.png]]

![[Pasted image 20230426172719.png]]

![[Pasted image 20230426172729.png]]

![[Pasted image 20230426172739.png]]

# Graphics Pipeline

![[Pasted image 20230426172804.png]]

![[Pasted image 20230426172817.png]]

![[Pasted image 20230426172826.png]]

![[Pasted image 20230426172837.png]]

![[Pasted image 20230426172848.png]]

![[Pasted image 20230426172900.png]]

# Texture Mapping

![[Pasted image 20230426173006.png]]

![[Pasted image 20230426173018.png]]

![[Pasted image 20230426173031.png]]

# Bilinear Interpolation

![[Pasted image 20230426173129.png]]


![[Pasted image 20230426173140.png]]

![[Pasted image 20230426173151.png]]

![[Pasted image 20230426173204.png]]

![[Pasted image 20230426173214.png]]

![[Pasted image 20230426173227.png]]

# Environment Mapping and Lighting

![[Pasted image 20230426173306.png]]

![[Pasted image 20230426173325.png]]

# Bump Mapping

![[Pasted image 20230426173353.png]]

![[Pasted image 20230426173405.png]]

# Displacement Mapping

![[Pasted image 20230426173421.png]]

# Implicit/Explicit Geo

![[Pasted image 20230426173454.png]]

# Convex Hull

![[Pasted image 20230426173638.png]]

# Piecewise Bezier

![[Pasted image 20230426173657.png]]

![[Pasted image 20230426173715.png]]

# Mesh Ops

![[Pasted image 20230426173933.png]]

# Loop Subdivision

![[Pasted image 20230426173904.png]]

# Simplification by Collapse

![[Pasted image 20230426174034.png]]
