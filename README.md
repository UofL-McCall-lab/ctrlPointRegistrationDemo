# ctrlPointRegistrationDemo
Applies fitgeotrans w/similarity in MATLAB to one moving image over one fixed image.
cpselect usage notes:
For this demo, you need at least three pairs of points

Left click places a point on one image, click the same "feature" on the
other image to finish a pair (indicated by the same integer identifying
pairs)

By checking the lock ratio checkbox you can zoom both in/out at the same
level to more precisely place control points.

When finished, in the cpselect tool go to file -> close control point selection tool

If multiple images need the same exact transform, it is trivial to take
myTransform and apply it to many images in a loop

Generate transform and align images. See 'transform type' table of the fitgeotrans() function page.

Transformation info:
Transformation type controls the minimum number of pairs needed to generate transform.
In this case, there must be at least three pairs to generate a transform ('similarity')

See which kind of transformation you need and change accordingly (is there
warping between the images or is just translation, rotation, and scaling
all that is needed? etc etc).
