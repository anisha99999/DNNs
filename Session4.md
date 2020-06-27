# DNNs

How many layers to use for a given image size: It will depend upon the kernel size. If the image size is nxn and kernel size is fxf then no of layers is usually (n+1)/(f-1)

MaxPooling: It is used to reduce the image size usually by half by usung 2x2 matrix. This reduces the total number of layers after convolution.

1x1 Convolutions : This matrix is used when we need to reduce the number of channels. So instead of using higher order kernel and increase computancy 1x1 kernel is used. 

3x3 Convolutions : It is the most common kernel size used for convolution. 

Receptive Field: It is the amount of info a layer has stored after its convolution. For eg for an image one convlution by 3x3 kernel gives a layer  whose receptive field is 3x3. After another convolution by 3x3 kernel the new layer has the receptive field of 5x5.

SoftMax: It is probability like process to normalize the last obtained layer for faster loss propagation during iteration. This also makes computation faster.

Learning Rate: It is the parameter in the program to optimise the step size iteration of the model. Smaller step size means longer computation time and slower model at it will take longer time to reach the minimum loss propagation and faster LR means model might skip that minima

Kernels and how do we decide the number of kernels : Kernel is a filter which is used for convolution with the image and get various layers. No of kernels is determined by the number of channels in the image or increase/decrease no of channels in the layers. 

Batch Normalization: It is the process of normalization of a layer for faster computation and better accuracy. Each layer after every convolution changes its distribution so normalizing after every convolution is ideal for better performance.   

Image Normalization: Image is normalized before its convolution else its distribuation will be very varied and so the computation/learning rate will be slower and accuracy slower. 

Position of MaxPooling: Maxpooling is usually done after convolution of a layer. It can be be done several times in the convolution network.

Concept of Transition Layers: Transition layers are the layers in between the convolutional network added to reduce the image size and reduce the no of channels. This reduces the complexity of the model.

Position of Transition Layer: It is usually after the convolution layer and after convolution the layer has maximum no of channels.

Number of Epochs and when to increase them: It is the no of times the model will run through all the training datasets. When the train data set is too complex it can be increased but careful enough to avoid overfitting.

DropOut:It is the process in which model selects some weights and drops the rest. It is to make model more accurate so that the model doesnt focus only on few predominant features but on random features.

When do we introduce DropOut, or when do we know we have some overfitting: When the model doesnt predict but memorises the outcome of the dataset so the accuracy vastly drops when the model is run on a new dataset.

The distance of MaxPooling from Prediction ??

The distance of Batch Normalization from Prediction ??

When do we stop convolutions and go ahead with a larger kernel or some other alternative (which we have not yet covered)

How do we know our network is not going well, comparatively, very early : The first epoch itself is giving higher losses and taking longer time

Batch Size, and effects of batch size: Batch sizes such as 32,64 is usually used when the datasets are large to be run in one epoch. 

When to add validation checks : ??

LR schedule and concept behind it : LR is the determine the optimised step size for the model to learn the data set

Adam vs SGD

etc (you can add more if we missed it here)
