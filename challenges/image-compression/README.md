# Image Compression

Challenge:
Assume you are passed an array of bytes representing a consecutive series of images (no padding).
Assume each image is 100 x 100 pixels and that each pixel is represented by 1 byte (so each image is exactly 10k bytes in length).
Imagine each image, is a shape (square, diamond, triangle, etc.) and can repeat an indefinite amount of times.
Each byte can be either 1 or 0 to represent either a black or a white pixel.
Write a compression algorithm that will compress the bytes in a way where they can reconstruct the original array.

eg. [1, 1, 1, 0, 1, 1, 0, 0, ....]
