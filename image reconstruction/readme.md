# Image Reconstruction, Compressed Sensing

Welcome, Here is the code that does image reconstruction via compressed sensing.

Thus far, image reconstruction via  a universal basis worked the following way.

You take a high resolution image and fourier transform it; 

you throw most of the transform data away;

you inverse fourier it with the remaining data samples and you still have a decent reconstruction of the original image.

Via compressed sensing, due to advancements in sparse optimization and computing, we can do this inturn.

You take an incomplete measurement of the given image by masking many pixels.

the sparse representation of the given image that has least non-zero entries, that satisfies the mask constraint is sought and found via optimization solvers.

the reconstruction image is found via inverse fourier transform of the sparse representation.

The files in this repo do the following respectively.

1. The .ipynb file named "Making RBG Data out of Image", finds the fourier basis vector that when multiplied with the given image vector, gives its sparse notation.
2. "solving optimization.py"-from the incomplete measurement of the given image, the sparse representation that minimizes the 'first-norm' and satisfies the constraint is found via solving a well formulated optimization problem.
3. "RGB reconstruction.ipynb"-the reconstruction is thus found from the inverse fourier transform of the sparse representation.

RBG channel images are made out of a 100 x 100 pixel image for the purpose of reconstruction soon after, via the algorithm made earlier.
The content made can be accessed [here](https://drive.google.com/drive/u/1/folders/1sETCN0vasFGGWXO63an9JtbTjfZRZzgF)
