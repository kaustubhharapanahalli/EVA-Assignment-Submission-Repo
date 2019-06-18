Assignment 7A - Kaustubh M Harapanahalli

# Calculating RF for GoogleNet model

In the table below, the details which are put up are the type of layer, the kernel size, the stride value, the output image size, the receptive field and jump in and jump out



#### RF Table

| Layer        | Kernel Size | Strides | Image Size | Receptive Field | Jump In | Jump Out |
| ------------ | ----------- | ------- | ---------- | --------------- | ------- | -------- |
| input        | 1           | 0       | 224        | 1               | 1       | 1        |
| convolution  | 7           | 2       | 112        | 7               | 1       | 2        |
| max pool     | 3           | 2       | 56         | 11              | 2       | 4        |
| convolution  | 1           | 1       | 56         | 11              | 4       | 4        |
| convolution  | 3           | 1       | 56         | 19              | 4       | 4        |
| max pool     | 3           | 2       | 28         | 27              | 4       | 8        |
| 3a inception | 5           | 1       | 28         | 59              | 8       | 8        |
| 3b inception | 5           | 1       | 28         | 91              | 8       | 8        |
| max pool     | 3           | 2       | 14         | 107             | 8       | 16       |
| 4a inception | 5           | 1       | 14         | 171             | 16      | 16       |
| 4b inception | 5           | 1       | 14         | 235             | 16      | 16       |
| 4c inception | 5           | 1       | 14         | 299             | 16      | 16       |
| 4d inception | 5           | 1       | 14         | 363             | 16      | 16       |
| 4e inception | 5           | 1       | 14         | 427             | 16      | 16       |
| max pool     | 3           | 2       | 7          | 459             | 16      | 32       |
| 5a inception | 5           | 1       | 7          | 587             | 32      | 32       |
| 5b inception | 5           | 1       | 7          | 715             | 32      | 32       |
| Average Pool | 7           | 1       | 1          | 907             | 32      | 32       |



**The global receptive field of GoogLeNet is 907.**

