
#graphics 

# View Transform

## Definition

Like a camera, has three parts:

1. Model Transform
2. View Transform
3. Projection Transform

## ModelView Transformation

Position: e->

Gaze: g-hat

Local up: t-hat, perpendicular to gaze

If all objects move together, view is the same.

Camera is transformed by: 

$$ M_{view} $$  

## M_view In Math

$$ M_{view} = R_{view}T_{view} $$

$$ T = \begin{pmatrix}   1 & 0 & 0 & -x_e\\ 0 & 1 & 0 & -y_e\\   0 & 0 & 1 & -z_e\\ 0 & 0 & 0 & 1  \end{pmatrix}
$$
