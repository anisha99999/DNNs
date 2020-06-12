# DNNs
Number of parameters are different because they is an additional step of linearization in pytorch leading to additional parameters. Since the  
filter is 
Keras parameters : _________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_185 (Conv2D)          (None, 18, 18, 32)        3904      
_________________________________________________________________
max_pooling2d_80 (MaxPooling (None, 9, 9, 32)          0         
_________________________________________________________________
conv2d_186 (Conv2D)          (None, 3, 3, 10)          15690     
_________________________________________________________________
max_pooling2d_81 (MaxPooling (None, 1, 1, 10)          0         
_________________________________________________________________
flatten_60 (Flatten)         (None, 10)                0         
_________________________________________________________________
activation_60 (Activation)   (None, 10)                0         
=================================================================
Total params: 19,594
Trainable params: 19,594
Non-trainable params: 0

PyTorch:

19704
[3872, 32, 15680, 10, 100, 10]
