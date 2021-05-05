# Hiding inside image

## What is a digital image?
The **digital image** is a finite set of digital values, called pixels. Pixels are the smallest individual element of an image, holding values that represent the brightness of a given color at any specific point. 
![digital image!](/images/4_digital.png "digital image")

This method only works on **Lossless-compression** images, which means that the files are stored in a compressed format, but that this compression does not result in the data being lost or modified, PNG, TIFF, and BMP as an example, are lossless-compression image file formats.

## Pixel concept and color models
Pixels are the smallest individual element of an image
Each pixel contains three values which are (*Red*, *Green*, *Blue*), these values (range from 0-255), in other words, they are 8-bit values.

![Pixel!](/images/6_pixel.png "Pixel")

For example, a value of 225 is 11100001
![Least Significant Bit!](/images/3_lsb-a.png "Least Significant Bit")


## Least Significant Bit Steganography
**L**east **S**ignificant **B**it **(LSB)** is a technique in which the last bit of each pixel is modified and replaced with the secret message’s data bit.
![significant bit!](/images/7_lsb.jpeg "Least Significant Bit")

![Least Significant Bit!](/images/3_lsb-b.png "Least Significant Bit")


### How LSB technique works?
Let's take an example of how this technique works:
1. hide the message **"hi"** into a 4x4 image, here are the example image pixel values:
```
[(225, 12, 99), (155, 2, 50), (99, 51, 15), (15, 55, 22),
(155, 61, 87), (63, 30, 17), (1, 55, 19), (99, 81, 66),
(219, 77, 91), (69, 39, 50), (18, 200, 33), (25, 54, 190)]
```
2. looking at the ASCII Table, and convert this message into decimal values and then into binary:
```
0110100 0110101
```
3. Now, iterate over the pixel values one by one, after converting them to binary, then replace each least significant bit with that message bits sequentially (e.g 225 is 11100001, we replace the last bit, the bit in the right (1) with the first data bit (0) and so on).
Here is the resulting pixel values:
```
[(224, 13, 99),(154, 3, 50),(98, 50, 15),(15, 54, 23),
(154, 61, 87),(63, 30, 17),(1, 55, 19),(99, 81, 66),
(219, 77, 91),(69, 39, 50),(18, 200, 33),(25, 54, 190)]
```
