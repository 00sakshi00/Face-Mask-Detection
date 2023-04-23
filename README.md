# Face-Mask-Detection

In this project CNN is used to detect wether person in image is wearing mask or not. This is very helpful during pandemics to detect and alert people to wear masks.

## CNN layers and working

### Input Layers: 
It’s the layer in which we give input to our model. In CNN, Generally, the input will be an image or a sequence of images. This layer holds the raw input of the image with width 128, height 128, and depth 3.

### Convolutional Layers: 
This is the layer, which is used to extract the feature from the input dataset. It applies a set of learnable filters known as the kernels to the input images. The filters/kernels are smaller matrices usually 2×2, 3×3, or 5×5 shape. it slides over the input image data and computes the dot product between kernel weight and the corresponding input image patch. The output of this layer is referred ad feature maps.

### Activation Layer: 
By adding an activation function to the output of the preceding layer, activation layers add nonlinearity to the network. it will apply an element-wise activation function to the output of the convolution layer.

### Pooling layer: 
This layer is periodically inserted in the covnets and its main function is to reduce the size of volume which makes the computation fast reduces memory and also prevents overfitting. Two common types of pooling layers are max pooling and average pooling.

### Flattening: 
The resulting feature maps are flattened into a one-dimensional vector after the convolution and pooling layers so they can be passed into a completely linked layer for categorization or regression.

### Fully Connected Layers: 
It takes the input from the previous layer and computes the final classification or regression task.

### Output Layer: 
The output from the fully connected layers is then fed into a logistic function for classification tasks like sigmoid or softmax which converts the output of each class into the probability score of each class.

![](https://editor.analyticsvidhya.com/uploads/719641_uAeANQIOQPqWZnnuH-VEyw.jpeg)