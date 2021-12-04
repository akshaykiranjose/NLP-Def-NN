Welcome, Here is the code that does image reconstruction via compressed sensing.
Thus far, image reconstruction via  a universal basis worked this way.
You take a high resolution image and fourier transform it $x\Phix$; 
you throw 95% of the transform data away; 
you inverse fourier it with the remaining data samples and you still have a decent reconstruction of the original image.

Via compressed sensing, due to advancements in sparse optimization and computing, we can do this inturn.
You find a sparse representation of the given image (an incomplete measurement $y=Cx$)
fourier transform it 



1. Given the image(100 * 100 for brevity), the .ipynb file named "Making RBG Data out of Image", finds the fourier basis vector that when multiplied with the sparse  
takes the incomplete image given as part of the project and solves the sparse oprtimization problem using scipy.optimize and finds the sparse matrix.
Proceeds with finding the matrix that can be used to get back the original, or an attempt at getting that via inverse Fourier transformation.

RBG channel images are made out of a 100 x 100 pixel image for the purpose of reconstruction soon after, via the algorithm made earlier.
The content made can be accessed [here](https://drive.google.com/drive/u/1/folders/1sETCN0vasFGGWXO63an9JtbTjfZRZzgF)

The file named Problem 5, takes the rgb channel data made earlier and reconstructs a color image from it.
