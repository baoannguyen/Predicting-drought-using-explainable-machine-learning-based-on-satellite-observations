# Astronomial Image Data 

## FITS

FITS stands for "Flexible Image Transport System" and is the standard astronomical data format endorsed by both NASA and the IAU. FITS is much more than an image format (such as JPG or GIF) and is primarily designed to store scientific data sets consisting of multi-dimensional arrays (1-D spectra, 2-D images or 3-D data cubes) and 2-dimensional tables containing rows and columns of data.

A FITS file consists of one or more Header + Data Units (HDUs), where the first HDU is called the "Primary HDU", or "Primary Array". The primary array contains an N-dimensional array of pixels, such as a 1-D spectrum, a 2-D image, or a 3-D data cube. Five different primary data types are supported: unsigned 8-bit bytes, 16 and 32-bit signed integers, and 32 and 64-bit single or double precision floating point reals. FITS can also store 16 and 32-bit unsigned integers.

Any number of additional HDUs may follow the primary array; these additional HDUs are called FITS "extensions". There are currently 3 types of extensions defined by the FITS Standard:

1. Image Extension - a N-dimensional array of pixels, like in a primary array
2. ASCII Table Extension - rows and columns of data in ASCII character format
3. Binary Table Extension - rows and columns of data in binary representation

![Screenshot 2022-03-08 173910](https://user-images.githubusercontent.com/57124909/157223326-24b398a0-c5dc-4e3d-850c-4006f904408a.png)

FITS data are opened by astropy Python package

# Image Processing

The unprocessed image: 

![Unprocessed_fig](https://user-images.githubusercontent.com/57124909/159757399-1a366e5e-05eb-48a7-80d8-cff3c763b4ab.png)

There are four fundamnetal processing: image representation, image enhacement, image reconstruction

## Image enhancement

1. Histogram equalization

![Hist_equal](https://user-images.githubusercontent.com/57124909/159764843-8d95cd92-9bda-4709-aacd-3fe2c6b8dd26.png)

2. Constrast Enhancement
