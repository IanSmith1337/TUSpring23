#graphics 

# Perspective

## Important Note

$$ (x, y, z, 0), (kx, ky, kz, k \not= 0), (xz, yz, z^2, z\not=0) $$  

all of above equal

$$ (1, 0, 0) $$

## Perspective to [[Orthographic]] Matrix

$$ \begin{pmatrix}   n & 0 & 0 & 0 \\ 0 & n & 0 & 0\\   0 & 0 & n+f & -nf\\ 0 & 0 & 1 & 0  \end{pmatrix}
$$

## Perspective Projection Matrix

$$ M_{ortho} \bullet \begin{pmatrix}   n & 0 & 0 & 0 \\ 0 & n & 0 & 0\\   0 & 0 & n+f & -nf\\ 0 & 0 & 1 & 0  \end{pmatrix}
$$
