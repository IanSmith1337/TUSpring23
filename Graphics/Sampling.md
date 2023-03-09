
#graphics 

# Sampling

## Definition

Nothing in [[Computer Graphics]] is continuous. Sampling determines if a [[Pixel]] has a certain value on a [[Screen]]. Implementation of [[Rasterization]].

## Types

[[Bounding Box]]
[[Incremental Triangle Traversal]]

## Using Cross Products to Determine Interior

Using p0 and p1 (two points of triangle) then drawing a line from p0 to the point to evaluate: if cross product shows that the point is in the direction of interior and overlapping on all three sides of triangle, then it is inside. 
