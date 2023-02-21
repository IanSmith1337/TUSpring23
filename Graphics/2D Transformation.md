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

S(0.5, 1.0):

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

$$r(theta):$$

$$ R_\theta = \begin{pmatrix}   cos(\theta) & -sin(\theta)\\   sin(\theta) & cos(\theta)  \end{pmatrix}
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
