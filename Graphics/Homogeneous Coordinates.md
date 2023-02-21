
#graphics 

# Homogeneous Coordinates

## Usage

Used in [[2D Transformation]].

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

$$\begin{pmatrix}   x\\   y\\ w   \end{pmatrix}$$ is the 2D Point

$$\begin{pmatrix}   x/w\\   y/w\\ 1   \end{pmatrix}$$

when w ≠ 0
