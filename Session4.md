# DNNs

How many layers to use for a given image size: It will depend upon the kernel size. If the image size is nxn and kernel size is fxf then no of layers is usually (n+1)/(f-1)
MaxPooling: It is used to reduce the image size usually by half by usung 2x2 matrix. This reduces the total number of layers after convolution.
1x1 Convolutions : This matrix is used when we need to reduce the number of channels. So instead of using higher order kernel and increase computancy 1x1 kernel is used. 
3x3 Convolutions : It is the most common kernel size used for convolution. 
Receptive Field: It is the amount of info a layer has stored after its convolution. For eg for 5x5 image one convlution by 3x3 kernel gives a 3x3 layer  whose receptive field is 3x3. After another convolution by 3x3 kernel gives a 1x1 layer whose receptive field is 5x5.
SoftMax: It is probability like process to normalize the last obtained layer for faster loss propagation during iteration. This also makes computation faster.
Learning Rate: It is the parameter in the program to optimise the step size iteration of the model. Smaller step size means longer computation time and slower model at it will take longer time to reach the minimum loss propagation and faster LR means model might skip that minima
Kernels and how do we decide the number of kernels : Kernel is a filter which is used for convolution with the image and get various layers. No of kernels is determined by the number of channels in the image or increase/decrease no of channels in the layers. 
Batch Normalization: It is the process of normalization of a layer for faster computation and better accuracy. Each layer after every convolution changes its distribution so normalizing after every convolution is ideal for better performance.   
Image Normalization: Image is normalized before its convolution else its distribuation will be very varied and so the computation/learning rate will be slower. 
Position of MaxPooling
Concept of Transition Layers
Position of Transition Layer
Number of Epochs and when to increase them
DropOut
When do we introduce DropOut, or when do we know we have some overfitting
The distance of MaxPooling from Prediction
The distance of Batch Normalization from Prediction
When do we stop convolutions and go ahead with a larger kernel or some other alternative (which we have not yet covered)
How do we know our network is not going well, comparatively, very early
Batch Size, and effects of batch size
When to add validation checks
LR schedule and concept behind it
Adam vs SGD
etc (you can add more if we missed it here)
