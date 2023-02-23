#graphics

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
