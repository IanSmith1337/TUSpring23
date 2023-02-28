#graphics 

# Orthographic

## Definition

Camera at origin (-Z look, Y up)

Drops Z coordinate


[[3D Transformation|Translate and scale]] resulting rectangle to canonical view within 

$$[-1, 1]^2$$

## Process

Given:

$$[l, r] \times [b, t] \times [f, n] $$  

and translating to:

$$ [-1, 1]^3 $$

1. Find center:

$$\frac{l+r}{2}, \frac{t+b}{2}, \frac{f+n}{2}$$

2. Transform matrix:

$$ T = \begin{pmatrix}   1 & 0 & 0 & -\frac{l+r}{2}\\ 0 & 1 & 0 & -\frac{t+b}{2}\\   0 & 0 & 1 & -\frac{f+n}{2}\\ 0 & 0 & 0 & 1  \end{pmatrix}
$$
