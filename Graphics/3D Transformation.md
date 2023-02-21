#graphics

# 3D Transformation

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

$$ R_x(\alpha) = \begin{pmatrix}   1 & 0 & 0 & 0\\ 0 & cos(\alpha) & -sin(\alpha) & 0\\   0 & sin(\alpha) & cos(\alpha) & 0\\ 0 & 0 & 0 & 1  \end{pmatrix}
$$

$$ R_y(\alpha) = \begin{pmatrix}   cos(\alpha) & 0 & sin(\alpha) & 0\\ 0 & 1 & 0 & 0\\   -sin(\alpha) & 0 & cos(\alpha) & 0\\ 0 & 0 & 0 & 1  \end{pmatrix}
$$
$$ R_z(\alpha) = \begin{pmatrix}   cos(\alpha) & -sin(\alpha) & 0 & 0\\ sin(\alpha) & cos(\alpha) & 0 & 0\\ 0 & 0 & 1 & 0\\ 0 & 0 & 0 & 1  \end{pmatrix}
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
