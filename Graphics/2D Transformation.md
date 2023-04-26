#graphics

# 2D Transformation

## Scale

S(x):

$$ 
x' = sx
$$

$$ 
y' = sy
$$

S(x, y):

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