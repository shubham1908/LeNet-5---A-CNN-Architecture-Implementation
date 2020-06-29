# LeNet-5---A-Classic-CNN-Architecture-Implementation

## LeNet-5 Architecture
<p>The LeNet-5 architecture consists of two sets of convolutional and average pooling layers, followed by a flattening convolutional layer, then two fully-connected layers and finally a softmax classifier.</p>

### First Layer:

The input for LeNet-5 is a 32×32 grayscale image which passes through the first convolutional layer with 6 feature maps or filters having size 5×5 and a stride of one. The image dimensions changes from 32x32x1 to 28x28x6.

### Second Layer:

Then the LeNet-5 applies average pooling layer or sub-sampling layer with a filter size 2×2 and a stride of two. The resulting image dimensions will be reduced to 14x14x6.

### Third Layer:
Next, there is a second convolutional layer with 16 feature maps having size 5×5 and a stride of 1.

### Fourth Layer:

The fourth layer (S4) is again an average pooling layer with filter size 2×2 and a stride of 2. This layer is the same as the second layer (S2) except it has 16 feature maps so the output will be reduced to 5x5x16.

### Fifth Layer:

The fifth layer (C5) is a fully connected convolutional layer with 120 feature maps each of size 1×1. Each of the 120 units in C5 is connected to all the 400 nodes (5x5x16) in the fourth layer S4.

### Sixth Layer:

The sixth layer is a fully connected layer (F6) with 84 units.

### Output Layer:

Finally, there is a fully connected softmax output layer ŷ with 10 possible values corresponding to the digits from 0 to 9.


![LeNet-5](Images/LeNEt_Summary_Table.jpg?raw=true "LeNet-5")
