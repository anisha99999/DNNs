# DNNs

1. Channels are features describing Layers and kernels are features describing filters. In 2D kernels and filters are the same but in 3D filters are formed by multiple kernels stacked together. Each kernel when applied into an input channel generates one output channel of the layer.

2.Usually Kernels are preferred to to be matrices such as 1x1,3x3,5x5 due to symmetry from its origin pixel. 3x3 is the smallest size odd matrix which gives maximum no of layers with less weight(3x3=9 ,5x5=25). So more no of layers means more features and information in it and with less no of weight makes the computations simpler and more efficient. 

3.  199x199 matrix will convulate 99 times with 3x3 matrix to get 1x1

199x199 | 3x3 > 197x197
197x197 | 3x3 > 195x195
.......................
5x5 | 3x3 > 3x3
3x3 | 3x3 > 1x1



