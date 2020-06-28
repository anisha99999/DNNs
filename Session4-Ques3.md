# DNNs


Conv Network: 
Conv1 : 28x28x1    Kernel 11x11x32     #18x18x32
Max pool …. 9x9x32
Conv2 .. 9x9x3…kernel 5x5x10 ….#5x5x10
Conv3… 5x5x10… kernel 5x5x10…  #1x1x10
No of Parameters: 
14574
[3872, 32, 8000, 10, 10, 10, 2500, 10, 10, 10, 100, 10]

Code1: 
Increase in LR without RELU 
1	# Network when LR=0.01 and No RELU	Epoch 10 - Time Taken: 0.2571983893712362, Training loss: 0.1724029005274796 - Train Accuracy: 0.9624 Test Accuracy: 0.9605
2	# Network when LR=0.01 and No RELU and Softmax	Epoch 10 - Time Taken: 0.26559211015701295, Training loss: 2.3142302615810304 - Train Accuracy: 0.08856666666666667 Test Accuracy: 0.0889
3	# Network when LR=0.003 and No RELU 	Epoch 10 - Time Taken: 0.25654162565867106, Training loss: 0.07754499984504 - Train Accuracy: 0.9767666666666667 Test Accuracy: 0.9702



 
Code2:
Increase in LR +RELU

1	# Network when LR=0.01 and RELU on 1st Conv	Epoch 10 - Time Taken: 0.25247056086858116, Training loss: 0.09489980373761929 - Train Accuracy: 0.97415 Test Accuracy: 0.9658
2	# Network when LR=0.01 and RELU on 1st Conv and 2nd Conv	Epoch 10 - Time Taken: 0.2662894050280253, Training loss: 0.07959101371753063 - Train Accuracy: 0.9809833333333333 Test Accuracy: 0.9743
3	# Network when LR=0.001 and RELU on 1st Conv and 2nd Conv	Epoch 10 - Time Taken: 0.26407456398010254, Training loss: 0.03550192425801937 - Train Accuracy: 0.9896666666666667 Test Accuracy: 0.9884
4	# Network when LR=0.003 and RELU on 1st Conv and 2nd Conv	Epoch 10 - Time Taken: 0.2535722772280375, Training loss: 0.029473833334662004 - Train Accuracy: 0.9916 Test Accuracy: 0.9888


 
Code3: 
1	# Network when LR=0.001 and RELU on 1st Conv and 2nd Conv and BN	Epoch 10 - Time Taken: 0.28090558052062986, Training loss: 0.019724513620519434 - Train Accuracy: 0.9964666666666666 Test Accuracy: 0.9892
2	# Network when LR=0.001 and RELU on 1st Conv and BN	Epoch 10 - Time Taken: 0.27307591438293455, Training loss: 0.02255102486085536 - Train Accuracy: 0.9956166666666667 Test Accuracy: 0.9902
3	# Network when LR=0.003 and RELU on 1st Conv and BN	Epoch 10 - Time Taken: 0.2715452273686727, Training loss: 0.020411519389321554 - Train Accuracy: 0.9948666666666667 Test Accuracy: 0.9913
4	# Network when LR=0.003 and RELU on 1st Conv and BN and Dropout	Epoch 10 - Time Taken: 0.27753301461537677, Training loss: 0.039647170217401946 - Train Accuracy: 0.9891333333333333 Test Accuracy: 0.9863
Increase in LR +RELU+BN (Dropout reduces accuracy)




 
Code 4:
Increase in LR+RELU+BN+Batch size
1	# Network when LR=0.003 and RELU on 1st Conv and BN and Batchsize=32	Epoch 10 - Time Taken: 0.40185822248458863, Training loss: 0.02279373536904653 - Train Accuracy: 0.9936833333333334 Test Accuracy: 0.9907
2	# Network when LR=0.003 and RELU on 1st Conv and 2nd Conv BN and Batchsize=128	Epoch 10 - Time Taken: 0.22394582827885945, Training loss: 0.02045799159943295 - Train Accuracy: 0.99565 Test Accuracy: 0.9913

 


